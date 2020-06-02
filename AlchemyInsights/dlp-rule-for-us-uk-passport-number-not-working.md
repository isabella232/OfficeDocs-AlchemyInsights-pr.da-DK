---
title: DLP-regel for pasnummer i USA/Storbritannien fungerer ikke
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 3d3b7dc2d9510376bc9eef6ec69b87ad7c681b05
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507292"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemer med DLP - USA/Storbritannien pasnumre

**Vigtigt**: I disse hidtil usete tider bestræber vi os på at sikre, at SharePoint Online- og OneDrive-tjenesterne fastholder sin høje tilgængelighed. Hvis du ønsker flere oplysninger, skal du besøge [Midlertidige funktionsjusteringer i SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP problemer med USA / UK pasnumre**

Har du problemer med **Forebyggelse af datatab (DLP),** der ikke arbejder for indhold, der indeholder et **amerikansk/britisk pasnummer,** når du bruger en DLP-følsom informationstype i O365? Hvis det er tilfældet, skal du sørge for, at dit indhold indeholder de nødvendige oplysninger om, hvad DLP-politikken søger efter, når den evalueres.
  
For en politik for pasnummer i **USA/Storbritannien,** der er konfigureret med et konfidensniveau på 75 %, evalueres følgende og skal registreres, for at reglen kan udløses
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Ni cifre

- **[Mønster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Ni cifre i træk

- **[Kontrolsum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nej, der er ingen Checksum

- **[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** En DLP-politik er 75 % sikker på, at den registreres denne type følsomme oplysninger, hvis den er i nærheden af 300 tegn:

  - Funktionen Func_usa_uk_passport finder indhold, der svarer til mønsteret.

  - Der blev fundet et nøgleord fra Keyword_passport.

    For eksempel vil følgende prøve udløse for **den amerikanske / britiske pas nummer** politik: US Passport nummer 123456789

Du kan finde flere oplysninger om, hvad der kræves for at få registreret et amerikansk/britisk passport-nummer for dit indhold, i følgende afsnit i denne artikel: [Hvad de følsomme informationstyper søger efter amerikansk/britisk passport-nummer](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Brug af en anden indbygget følsom oplysningstype i følgende artikel for at få oplysninger om, hvad der kræves til andre typer: [Hvad de følsomme oplysninger søger efter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  