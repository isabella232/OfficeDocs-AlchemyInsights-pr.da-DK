---
title: DLP-regel for SSN virker ikke
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b92d122b774d97cd2e44cc0880dc5001065b57cc
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/24/2019
ms.locfileid: "29464668"
---
Har du problemer med **Data tab forebyggelse (DLP)** ikke arbejder for indhold, der indeholder et **Personnummer (SSN)** , når du bruger en type af følsomme oplysninger i Office 365? Hvis det er tilfældet, skal du sørge for dit indhold indeholder de nødvendige oplysninger til hvad søger DLP-Gruppepolitik. 
  
For eksempel en SSN-politik, der er konfigureret med et konfidensniveau på 85%, følgende evalueres, og skal registreres for reglen, der udløser:
  
- **[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 cifre, hvilket kan være i en formateret eller uformateret mønster 
    
- **[Mønster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Fire funktioner se efter SSNs i fire forskellige mønstre: 
    
  - Func_ssn finder SSNs med pre-2011 stærk formatering, der er formateret med bindestreger eller mellemrum (ddd-dd-dddd eller ddd dd dddd)
    
  - Func_unformatted_ssn finder SSNs med pre-2011 stærk formatering, der er formateret som ni på hinanden følgende cifre (ddddddddd)
    
  - Func_randomized_formatted_ssn finder indlæg 2011-SSNs, der er formateret med bindestreger eller mellemrum (ddd-dd-dddd eller ddd dd dddd)
    
  - Func_randomized_unformatted_ssn finder indlæg 2011-SSNs, der er formateret som ni på hinanden følgende cifre (ddddddddd)
    
- **[Kontrolsum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nej, der er ingen kontrolsum 
    
- **[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** En DLP-politik er 85% sikker på, at det har fundet denne type af følsomme oplysninger, hvis, inden for en afstand af 300 tegn: 
    
  - [Funktionen Func_ssn](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) søger efter indhold, der svarer til mønsteret. 
    
  - Der findes et nøgleord fra [Keyword_ssn](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) . Indeholder eksempler på nøgleord: *Social sikring, Social sikring #, Soc sekund, SSN* . For eksempel vil udløse følgende eksempel for DLP SSN-politik: **SSN: 489-36-8350**
    
Yderligere oplysninger om, hvad der kræves for SSNs til at blive registreret til dit indhold, kan du se følgende afsnit i denne artikel: [Hvad den følsomme oplysningstyper Søg efter SSNs](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Bruge en anden indbygget følsomme oplysninger, se følgende artikel for at få oplysninger om hvad der kræves for andre typer: [Hvad den følsomme oplysningstyper søge efter](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

