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
ms.openlocfilehash: c63e814059c897531109aa78725e9811b311fb27
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931256"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemer med DLP - PASnumre i USA/STORBRITANNIEN

**Vigtigt**: Mange SharePoint Online- og OneDrive-kunder kører forretningskritiske programmer mod den tjeneste, der kører i baggrunden. Disse omfatter indholdsmigrering, Forebyggelse af datatab (DLP) og sikkerhedskopieringsløsninger. I disse hidtil usete tider tager vi skridt til at sikre, at SharePoint Online- og OneDrive-tjenester forbliver meget tilgængelige og pålidelige for dine brugere, der er afhængige af tjenesten mere end nogensinde før i scenarier for fjernarbejde.

Til støtte for dette mål har vi implementeret strammere begrænsningsgrænser for baggrundsapps (migrering, DLP og backupløsninger) i dagtimerne på hverdage. Du bør forvente, at disse apps vil opnå meget begrænset gennemløb i disse tider. I løbet af aftenen og i weekenden for regionen vil tjenesten dog være klar til at behandle en betydeligt større mængde anmodninger fra baggrundsapps.

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
  