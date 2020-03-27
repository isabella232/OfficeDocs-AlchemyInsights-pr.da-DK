---
title: DLP-regel for SSN fungerer ikke
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
ms.openlocfilehash: 4ec0df9d4954a8c65f0c34188d285dd8cf44a4f2
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977300"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="de799-102">DLP problemer med cpr-numre</span><span class="sxs-lookup"><span data-stu-id="de799-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="de799-103">**Vigtigt:** I disse hidtil usete tider tager vi skridt til at sikre, at SharePoint Online- og OneDrive-tjenester forbliver meget tilgængelige – Besøg [midlertidige sharepoint onlinefunktionsjusteringer](https://aka.ms/ODSPAdjustments) for at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="de799-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="de799-104">**DLP problemer med SSNs**</span><span class="sxs-lookup"><span data-stu-id="de799-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="de799-105">Har du problemer med **Forebyggelse af datatab (DLP),** der ikke fungerer for indhold, der indeholder et **CPR-nummer ,** når du bruger en følsom oplysningstype i Office 365?</span><span class="sxs-lookup"><span data-stu-id="de799-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="de799-106">Hvis det er tilfældet, skal du sørge for, at indholdet indeholder de nødvendige oplysninger om, hvad DLP-politikken søger.</span><span class="sxs-lookup"><span data-stu-id="de799-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="de799-107">For en SSN-politik, der er konfigureret med et konfidensniveau på 85 %, evalueres følgende f.eks., for at reglen udløses:</span><span class="sxs-lookup"><span data-stu-id="de799-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="de799-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 cifre, som kan være i et formateret eller uformateret mønster</span><span class="sxs-lookup"><span data-stu-id="de799-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="de799-109">**[Mønster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Fire funktioner søger SSN'er i fire forskellige mønstre:</span><span class="sxs-lookup"><span data-stu-id="de799-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="de799-110">Func_ssn finder SSN'er med stærk formatering før 2011, der er formateret med tankestreger eller mellemrum (ddd-ddddd OR ddd dd dddddd)</span><span class="sxs-lookup"><span data-stu-id="de799-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="de799-111">Func_unformatted_ssn finder SSN'er med stærk formatering før 2011, der ikke er formateret som ni på hinanden følgende cifre (ddddddddddd)</span><span class="sxs-lookup"><span data-stu-id="de799-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="de799-112">Func_randomized_formatted_ssn finder SSN'er efter 2011, der er formateret med tankestreger eller mellemrum (ddd-ddddd OR ddd dd dddddd)</span><span class="sxs-lookup"><span data-stu-id="de799-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="de799-113">Func_randomized_unformatted_ssn finder SSN'er efter 2011, der ikke er formateret som ni på hinanden følgende cifre (ddddddddddd)</span><span class="sxs-lookup"><span data-stu-id="de799-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="de799-114">**[Kontrolsum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nej, der er ingen Kontrolsum</span><span class="sxs-lookup"><span data-stu-id="de799-114">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="de799-115">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** En DLP-politik er 85 % sikker på, at den har registreret denne type følsomme oplysninger, hvis der ligger 300 tegn i nærheden af 300 tegn:</span><span class="sxs-lookup"><span data-stu-id="de799-115">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="de799-116">[Funktionen Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finder indhold, der svarer til mønsteret.</span><span class="sxs-lookup"><span data-stu-id="de799-116">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="de799-117">Der findes et nøgleord fra [Keyword_ssn.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn)</span><span class="sxs-lookup"><span data-stu-id="de799-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="de799-118">Eksempler på nøgleord omfatter: *Social Security, Social Security#, Soc Sec , SSN* .</span><span class="sxs-lookup"><span data-stu-id="de799-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="de799-119">Følgende eksempel udløser f.eks. **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="de799-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="de799-120">Du kan finde flere oplysninger om, hvad der kræves, for at SSN'er kan registreres for dit indhold, i følgende afsnit i denne artikel: [Hvad søger følsomme informationstyper efter SSN'er](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="de799-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="de799-121">Brug en anden indbygget type følsomme oplysninger finder du i følgende artikel for at få oplysninger om, hvad der kræves for andre typer: [Hvad de følsomme informationstyper søger efter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="de799-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  