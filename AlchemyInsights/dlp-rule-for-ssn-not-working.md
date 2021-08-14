---
title: DLP-regel for SSN fungerer ikke
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 3f30998fb3bc4c5442e4e1541b87d88ecd7df6eef3a50e719fa5014eb86af39c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004976"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP-problemer med CPR-numre

**Vigtigt**: I disse hidtil usete tider bestræber vi os på at sikre, at SharePoint Online- og OneDrive-tjenesterne fastholder sin høje tilgængelighed. Hvis du ønsker flere oplysninger, skal du besøge [Midlertidige funktionsjusteringer i SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP-problemer med SSN'er**

Har du problemer med forebyggelse af datatab **(DLP)** ikke for indhold, der indeholder et **CPR-nummer,** når du bruger en følsom oplysningstype i Microsoft 365? Hvis det er ja, skal du sørge for, at dit indhold indeholder de nødvendige oplysninger til det, som DLP-politikken søger efter. 
  
For en SSN-politik, der er konfigureret med et konfidensniveau på 85 %, evalueres følgende og skal registreres, for at reglen udløser:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 cifre, som kan være i et formateret eller uformateret mønster

- **[Mønster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Fire funktioner ser efter SSN'er i fire forskellige mønstre:

  - Func_ssn finder SSN'er med en stærk formatering før 2011, der er formateret med stiplede tankestreger eller mellemrum (ddd-dd-dddd ELLER ddd dd dddd)

  - Func_unformatted_ssn finder SSN'er med en stærk formatering (før 2011), der er formateret som ni fortløbende cifre (ddddddddd)

  - Func_randomized_formatted_ssn finder SSN'er efter 2011, der er formateret med tankestreger eller mellemrum (ddd-dd-dddd ELLER ddd dd dddd)

  - Func_randomized_unformatted_ssn finder SSN'er efter 2011, der er formateret som ni fortløbende cifre (ddddddddd)

- **[Kontrolsum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Nej, der er ingen Kontrolsum

- **[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** En DLP-politik er 85 % sikker på, at den har registreret denne type af følsomme oplysninger, inden for en afstand af 300 tegn:

  - Funktionen [finder Func_ssn,](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) der svarer til mønsteret.

  - Der er fundet [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) nøgleord. Eksempler på nøgleord omfatter:  *Social Security, Social Security#, Soc Sec , SSN*  . Følgende eksempel udløser f.eks. DLP SSN-politikken: **SSN: 489-36-8350**
  
Du kan finde flere oplysninger om, hvad der kræves for, at SSN'er registreres for dit indhold, i det følgende afsnit i denne artikel: Hvad typerne af følsomme oplysninger søger efter [SSN'er](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Ved hjælp af en anden indbygget type af følsomme oplysninger kan du se følgende artikel for at få oplysninger om, hvad der kræves til andre typer: Det, [som typerne](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) af følsomme oplysninger søger efter
  