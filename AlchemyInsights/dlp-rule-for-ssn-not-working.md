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
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/15/2019
ms.locfileid: "28282442"
---
<span data-ttu-id="2f446-p101">Har du problemer med **Data tab forebyggelse (DLP)** ikke arbejder for indhold, der indeholder et **Personnummer (SSN)** , når du bruger en type af følsomme oplysninger i Office 365? Hvis det er tilfældet, skal du sørge for dit indhold indeholder de nødvendige oplysninger til hvad søger DLP-Gruppepolitik.</span><span class="sxs-lookup"><span data-stu-id="2f446-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365? If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="2f446-104">For eksempel en SSN-politik, der er konfigureret med et konfidensniveau på 85%, følgende evalueres, og skal registreres for reglen, der udløser:</span><span class="sxs-lookup"><span data-stu-id="2f446-104">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="2f446-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 cifre, hvilket kan være i en formateret eller uformateret mønster</span><span class="sxs-lookup"><span data-stu-id="2f446-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span> 
    
- <span data-ttu-id="2f446-106">**[Mønster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Fire funktioner se efter SSNs i fire forskellige mønstre:</span><span class="sxs-lookup"><span data-stu-id="2f446-106">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span> 
    
  - <span data-ttu-id="2f446-107">Func_ssn finder SSNs med pre-2011 stærk formatering, der er formateret med bindestreger eller mellemrum (ddd-dd-dddd eller ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="2f446-107">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>
    
  - <span data-ttu-id="2f446-108">Func_unformatted_ssn finder SSNs med pre-2011 stærk formatering, der er formateret som ni på hinanden følgende cifre (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="2f446-108">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>
    
  - <span data-ttu-id="2f446-109">Func_randomized_formatted_ssn finder indlæg 2011-SSNs, der er formateret med bindestreger eller mellemrum (ddd-dd-dddd eller ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="2f446-109">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>
    
  - <span data-ttu-id="2f446-110">Func_randomized_unformatted_ssn finder indlæg 2011-SSNs, der er formateret som ni på hinanden følgende cifre (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="2f446-110">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>
    
- <span data-ttu-id="2f446-111">**[Kontrolsum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nej, der er ingen kontrolsum</span><span class="sxs-lookup"><span data-stu-id="2f446-111">**[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="2f446-112">**[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** En DLP-politik er 85% sikker på, at det har fundet denne type af følsomme oplysninger, hvis, inden for en afstand af 300 tegn:</span><span class="sxs-lookup"><span data-stu-id="2f446-112">**[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="2f446-113">[Funktionen Func_ssn](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) søger efter indhold, der svarer til mønsteret.</span><span class="sxs-lookup"><span data-stu-id="2f446-113">The [function Func_ssn](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span> 
    
  - <span data-ttu-id="2f446-p102">Der findes et nøgleord fra [Keyword_ssn](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) . Indeholder eksempler på nøgleord: *Social sikring, Social sikring #, Soc sekund, SSN* . For eksempel vil udløse følgende eksempel for DLP SSN-politik: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="2f446-p102">A keyword from [Keyword_ssn](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found. Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  . For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
    
<span data-ttu-id="2f446-117">Yderligere oplysninger om, hvad der kræves for SSNs til at blive registreret til dit indhold, kan du se følgende afsnit i denne artikel: [Hvad den følsomme oplysningstyper Søg efter SSNs](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="2f446-117">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="2f446-118">Bruge en anden indbygget følsomme oplysninger, se følgende artikel for at få oplysninger om hvad der kræves for andre typer: [Hvad den følsomme oplysningstyper søge efter](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="2f446-118">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

