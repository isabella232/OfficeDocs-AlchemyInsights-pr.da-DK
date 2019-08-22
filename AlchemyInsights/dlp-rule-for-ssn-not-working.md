---
title: DLP-regel for SSN virker ikke
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 757136c39700f12f40f839b29277a59b0e436f03
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529842"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="ceeff-102">DLP-problemer med CPR-numre</span><span class="sxs-lookup"><span data-stu-id="ceeff-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="ceeff-103">Har du problemer med **Data tab forebyggelse (DLP)** ikke arbejder for indhold, der indeholder et **Personnummer (SSN)** , når du bruger en type af følsomme oplysninger i Office 365?</span><span class="sxs-lookup"><span data-stu-id="ceeff-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="ceeff-104">Hvis det er tilfældet, skal du sørge for dit indhold indeholder de nødvendige oplysninger til hvad søger DLP-Gruppepolitik.</span><span class="sxs-lookup"><span data-stu-id="ceeff-104">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="ceeff-105">For eksempel en SSN-politik, der er konfigureret med et konfidensniveau på 85%, følgende evalueres, og skal registreres for reglen, der udløser:</span><span class="sxs-lookup"><span data-stu-id="ceeff-105">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="ceeff-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 cifre, hvilket kan være i en formateret eller uformateret mønster</span><span class="sxs-lookup"><span data-stu-id="ceeff-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="ceeff-107">**[Mønster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Fire funktioner se efter SSNs i fire forskellige mønstre:</span><span class="sxs-lookup"><span data-stu-id="ceeff-107">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="ceeff-108">Func_ssn finder SSNs med pre-2011 stærk formatering, der er formateret med bindestreger eller mellemrum (ddd-dd-dddd eller ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="ceeff-108">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="ceeff-109">Func_unformatted_ssn finder SSNs med pre-2011 stærk formatering, der er formateret som ni på hinanden følgende cifre (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="ceeff-109">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="ceeff-110">Func_randomized_formatted_ssn finder indlæg 2011-SSNs, der er formateret med bindestreger eller mellemrum (ddd-dd-dddd eller ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="ceeff-110">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="ceeff-111">Func_randomized_unformatted_ssn finder indlæg 2011-SSNs, der er formateret som ni på hinanden følgende cifre (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="ceeff-111">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="ceeff-112">**[Kontrolsum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nej, der er ingen kontrolsum</span><span class="sxs-lookup"><span data-stu-id="ceeff-112">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="ceeff-113">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** En DLP-politik er 85% sikker på, at det har fundet denne type af følsomme oplysninger, hvis, inden for en afstand af 300 tegn:</span><span class="sxs-lookup"><span data-stu-id="ceeff-113">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="ceeff-114">[Funktionen Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) søger efter indhold, der svarer til mønsteret.</span><span class="sxs-lookup"><span data-stu-id="ceeff-114">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="ceeff-115">Der findes et nøgleord fra [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) .</span><span class="sxs-lookup"><span data-stu-id="ceeff-115">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="ceeff-116">Indeholder eksempler på nøgleord: *Social sikring, Social sikring #, Soc sekund, SSN* .</span><span class="sxs-lookup"><span data-stu-id="ceeff-116">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="ceeff-117">For eksempel vil udløse følgende eksempel for DLP SSN-politik: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="ceeff-117">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="ceeff-118">Yderligere oplysninger om, hvad der kræves for SSNs til at blive registreret til dit indhold, kan du se følgende afsnit i denne artikel: [Hvad den følsomme oplysningstyper Søg efter SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="ceeff-118">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="ceeff-119">Bruge en anden indbygget følsomme oplysninger, se følgende artikel for at få oplysninger om hvad der kræves for andre typer: [Hvad den følsomme oplysningstyper søge efter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="ceeff-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  