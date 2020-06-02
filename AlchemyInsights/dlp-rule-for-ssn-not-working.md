---
title: DLP-regel for SSN fungerer ikke
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 35859bce89ef1ae9b6a9e706fc316b0ee6cd27d1
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507364"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP problemer med CPR-numre

**Vigtigt**: I disse hidtil usete tider bestræber vi os på at sikre, at SharePoint Online- og OneDrive-tjenesterne fastholder sin høje tilgængelighed. Hvis du ønsker flere oplysninger, skal du besøge [Midlertidige funktionsjusteringer i SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP-problemer med SSN'er**

Har du problemer med **forebyggelse af datatab (DLP),** der ikke arbejder for indhold, der indeholder et **SSN (Social Security Number),** når du bruger en følsom oplysningstype i Microsoft 365? Hvis det er tilfældet, skal du sørge for, at dit indhold indeholder de nødvendige oplysninger til, hvad DLP-politikken ser ud til. 
  
For en SSN-politik, der er konfigureret med et konfidensniveau på 85 %, evalueres følgende f.eks.
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 cifre, som kan være i et formateret eller uformateret mønster

- **[Mønster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Fire funktioner søger efter SSN'er i fire forskellige mønstre:

  - Func_ssn finder SSN'er med stærk formatering før 2011, der er formateret med streger eller mellemrum (dddd-ddddd ELLER ddd dd dd dddd)

  - Func_unformatted_ssn finder SSN'er med stærk formatering før 2011, der ikke er formateret som ni på hinanden følgende cifre (dddddddddddddddd)

  - Func_randomized_formatted_ssn finder SSN'er efter 2011, der er formateret med streger eller mellemrum (dddd-ddddd ELLER ddd dd dd dddd)

  - Func_randomized_unformatted_ssn finder SSN'er efter 2011, der ikke er formateret som ni på hinanden følgende cifre (ddddddddddd)

- **[Kontrolsum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Nej, der er ingen Checksum

- **[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** En DLP-politik er 85 % sikker på, at den registreres denne type følsomme oplysninger, hvis den er i nærheden af 300 tegn:

  - [Funktionen Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finder indhold, der svarer til mønsteret.

  - Der blev fundet et nøgleord fra [Keyword_ssn.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) Eksempler på søgeord omfatter: *Social Security, Social Security #, Soc Sec , SSN* . Følgende eksempel udløser **f.eks.**
  
Du kan finde flere oplysninger om, hvad der kræves for at opdage SSN'er for dit indhold, i følgende afsnit i denne artikel: [Hvad de følsomme oplysningstyper søger efter SSN'er](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Brug af en anden indbygget følsom oplysningstype i følgende artikel for at få oplysninger om, hvad der kræves til andre typer: [Hvad de følsomme oplysninger søger efter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  