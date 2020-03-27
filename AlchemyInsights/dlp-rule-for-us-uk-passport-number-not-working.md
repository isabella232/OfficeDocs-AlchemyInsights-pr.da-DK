---
title: DLP-regel for PASNUMMER MELLEM USA og STORBRITANNIEN fungerer ikke
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 534e258c31a9a71c618765511487487c53f455b5
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977100"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemer med DLP - PASnumre i USA/STORBRITANNIEN

**Vigtigt:** I disse hidtil usete tider tager vi skridt til at sikre, at SharePoint Online- og OneDrive-tjenester forbliver meget tilgængelige – Besøg [midlertidige sharepoint onlinefunktionsjusteringer](https://aka.ms/ODSPAdjustments) for at få flere oplysninger.

**DLP problemer med USA / UK pasnumre**

Har du problemer med **Forebyggelse af datatab (DLP),** der ikke fungerer for indhold, der indeholder et **amerikansk/britisk pasnummer,** når du bruger en DLP-følsom informationstype i O365? Hvis det er tilfældet, skal du sørge for, at indholdet indeholder de nødvendige oplysninger om, hvad DLP-politikken søger efter, når den evalueres.
  
For en **pasnummerpolitik** mellem USA og Storbritannien, der er konfigureret med et konfidensniveau på 75 %, evalueres følgende f.eks.
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Ni cifre

- **[Mønster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Ni cifre i træk

- **[Kontrolsum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nej, der er ingen Kontrolsum

- **[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** En DLP-politik er 75 % sikker på, at den har registreret denne type følsomme oplysninger, hvis der ligger 300 tegn i nærheden af 300 tegn:

  - Funktionen Func_usa_uk_passport finder indhold, der svarer til mønsteret.

  - Der findes et nøgleord fra Keyword_passport.

    Følgende eksempel udløser f.eks. **US/UK passport number**

Du kan finde flere oplysninger om, hvad der kræves, for at der kan registreres et PASSPORT-nummer mellem USA og Storbritannien for dit indhold, i følgende afsnit i denne artikel: [Hvad søger følsomme informationstyper efter passport-nummer](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number) mellem USA og Storbritannien
  
Brug en anden indbygget type følsomme oplysninger finder du i følgende artikel for at få oplysninger om, hvad der kræves for andre typer: [Hvad de følsomme informationstyper søger efter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  