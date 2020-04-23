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
ms.openlocfilehash: 5af843c2b70b5b2e1aaf82c9f01356546929d840
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43788696"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP problemer med cpr-numre

**Vigtigt**: I disse hidtil usete tider bestræber vi os på at sikre, at SharePoint Online- og OneDrive-tjenesterne fastholder sin høje tilgængelighed. Hvis du ønsker flere oplysninger, skal du besøge [Midlertidige funktionsjusteringer i SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP problemer med SSNs**

Har du problemer med **Forebyggelse af datatab (DLP),** der ikke fungerer for indhold, der indeholder et **CPR-nummer ( SSN),** når du bruger en følsom oplysningstype i Microsoft 365? Hvis det er tilfældet, skal du sørge for, at indholdet indeholder de nødvendige oplysninger om, hvad DLP-politikken søger. 
  
For en SSN-politik, der er konfigureret med et konfidensniveau på 85 %, evalueres følgende f.eks., for at reglen udløses:
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 cifre, som kan være i et formateret eller uformateret mønster

- **[Mønster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Fire funktioner søger SSN'er i fire forskellige mønstre:

  - Func_ssn finder SSN'er med stærk formatering før 2011, der er formateret med tankestreger eller mellemrum (ddd-ddddd OR ddd dd dddddd)

  - Func_unformatted_ssn finder SSN'er med stærk formatering før 2011, der ikke er formateret som ni på hinanden følgende cifre (ddddddddddd)

  - Func_randomized_formatted_ssn finder SSN'er efter 2011, der er formateret med tankestreger eller mellemrum (ddd-ddddd OR ddd dd dddddd)

  - Func_randomized_unformatted_ssn finder SSN'er efter 2011, der ikke er formateret som ni på hinanden følgende cifre (ddddddddddd)

- **[Kontrolsum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nej, der er ingen Kontrolsum

- **[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** En DLP-politik er 85 % sikker på, at den har registreret denne type følsomme oplysninger, hvis der ligger 300 tegn i nærheden af 300 tegn:

  - [Funktionen Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finder indhold, der svarer til mønsteret.

  - Der findes et nøgleord fra [Keyword_ssn.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) Eksempler på nøgleord omfatter: *Social Security, Social Security#, Soc Sec , SSN* . Følgende eksempel udløser f.eks. **SSN: 489-36-8350**
  
Du kan finde flere oplysninger om, hvad der kræves, for at SSN'er kan registreres for dit indhold, i følgende afsnit i denne artikel: [Hvad søger følsomme informationstyper efter SSN'er](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Brug en anden indbygget type følsomme oplysninger finder du i følgende artikel for at få oplysninger om, hvad der kræves for andre typer: [Hvad de følsomme informationstyper søger efter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  