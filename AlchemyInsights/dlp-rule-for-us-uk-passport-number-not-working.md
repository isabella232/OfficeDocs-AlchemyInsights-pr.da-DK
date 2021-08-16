---
title: DLP-regel for amerikanske/britiske pasnummer fungerer ikke
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 85e3ed7fdc221981de13ab6e2ada8adf2a3a80b40ff163981e047cc4a02a1514
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004940"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemer med DLP - AMERIKANSKE/britiske pasnumre

**Vigtigt**: I disse hidtil usete tider bestræber vi os på at sikre, at SharePoint Online- og OneDrive-tjenesterne fastholder sin høje tilgængelighed. Hvis du ønsker flere oplysninger, skal du besøge [Midlertidige funktionsjusteringer i SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP-problemer med amerikanske/britiske pasnumre**

Har du problemer med forebyggelse af datatab **(DLP)** ikke for indhold, der indeholder et **amerikansk/britisk pasnummer,** når du bruger en DLP-følsom oplysningstype i O365? Hvis det er ja, skal du sikre dig, at dit indhold indeholder de nødvendige oplysninger om, hvad DLP-politikken leder efter, når den evalueres.
  
Eksempelvis evalueres følgende, for en politik for pasnummer i **USA/Storbritannien,** der er konfigureret med et konfidensniveau på 75 %, og den skal registreres, for at reglen kan udløses
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Ni cifre

- **[Mønster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Ni fortløbende cifre

- **[Kontrolsum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nej, der er ingen Kontrolsum

- **[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** En DLP-politik er 75 % sikker på, at den har registreret denne type af følsomme oplysninger, inden for en afstand af 300 tegn:

  - Funktionen finder Func_usa_uk_passport, der svarer til mønsteret.

  - Der er fundet Keyword_passport nøgleord.

    Følgende eksempel udløser f.eks. en politik for pasnummer **i USA/Storbritannien:** USA's pasnummer 123456789

Du kan finde flere oplysninger om, hvad der kræves for at et amerikansk/britisk pasnummer kan findes for dit indhold, i det følgende afsnit i denne artikel: Hvad typerne af følsomme oplysninger søger efter et [amerikansk/britisk pasnummer](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Ved hjælp af en anden indbygget type af følsomme oplysninger kan du se følgende artikel for at få oplysninger om, hvad der kræves til andre typer: Det, [som typerne](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) af følsomme oplysninger søger efter
  