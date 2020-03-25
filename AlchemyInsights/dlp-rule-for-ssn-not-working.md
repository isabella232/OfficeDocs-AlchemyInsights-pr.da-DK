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
ms.openlocfilehash: 0b83a858975ffe1bb70f16a7452a13d57dff5340
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932515"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="0233d-102">DLP problemer med cpr-numre</span><span class="sxs-lookup"><span data-stu-id="0233d-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="0233d-103">**Vigtigt**: Mange SharePoint Online- og OneDrive-kunder kører forretningskritiske programmer mod den tjeneste, der kører i baggrunden.</span><span class="sxs-lookup"><span data-stu-id="0233d-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="0233d-104">Disse omfatter indholdsmigrering, Forebyggelse af datatab (DLP) og sikkerhedskopieringsløsninger.</span><span class="sxs-lookup"><span data-stu-id="0233d-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="0233d-105">I disse hidtil usete tider tager vi skridt til at sikre, at SharePoint Online- og OneDrive-tjenester forbliver meget tilgængelige og pålidelige for dine brugere, der er afhængige af tjenesten mere end nogensinde før i scenarier for fjernarbejde.</span><span class="sxs-lookup"><span data-stu-id="0233d-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="0233d-106">Til støtte for dette mål har vi implementeret strammere begrænsningsgrænser for baggrundsapps (migrering, DLP og backupløsninger) i dagtimerne på hverdage.</span><span class="sxs-lookup"><span data-stu-id="0233d-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="0233d-107">Du bør forvente, at disse apps vil opnå meget begrænset gennemløb i disse tider.</span><span class="sxs-lookup"><span data-stu-id="0233d-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="0233d-108">I løbet af aftenen og i weekenden for regionen vil tjenesten dog være klar til at behandle en betydeligt større mængde anmodninger fra baggrundsapps.</span><span class="sxs-lookup"><span data-stu-id="0233d-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="0233d-109">**DLP problemer med SSNs**</span><span class="sxs-lookup"><span data-stu-id="0233d-109">**DLP issues with SSNs**</span></span>

<span data-ttu-id="0233d-110">Har du problemer med **Forebyggelse af datatab (DLP),** der ikke fungerer for indhold, der indeholder et **CPR-nummer ,** når du bruger en følsom oplysningstype i Office 365?</span><span class="sxs-lookup"><span data-stu-id="0233d-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="0233d-111">Hvis det er tilfældet, skal du sørge for, at indholdet indeholder de nødvendige oplysninger om, hvad DLP-politikken søger.</span><span class="sxs-lookup"><span data-stu-id="0233d-111">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="0233d-112">For en SSN-politik, der er konfigureret med et konfidensniveau på 85 %, evalueres følgende f.eks., for at reglen udløses:</span><span class="sxs-lookup"><span data-stu-id="0233d-112">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="0233d-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 cifre, som kan være i et formateret eller uformateret mønster</span><span class="sxs-lookup"><span data-stu-id="0233d-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="0233d-114">**[Mønster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Fire funktioner søger SSN'er i fire forskellige mønstre:</span><span class="sxs-lookup"><span data-stu-id="0233d-114">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="0233d-115">Func_ssn finder SSN'er med stærk formatering før 2011, der er formateret med tankestreger eller mellemrum (ddd-ddddd OR ddd dd dddddd)</span><span class="sxs-lookup"><span data-stu-id="0233d-115">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="0233d-116">Func_unformatted_ssn finder SSN'er med stærk formatering før 2011, der ikke er formateret som ni på hinanden følgende cifre (ddddddddddd)</span><span class="sxs-lookup"><span data-stu-id="0233d-116">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="0233d-117">Func_randomized_formatted_ssn finder SSN'er efter 2011, der er formateret med tankestreger eller mellemrum (ddd-ddddd OR ddd dd dddddd)</span><span class="sxs-lookup"><span data-stu-id="0233d-117">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="0233d-118">Func_randomized_unformatted_ssn finder SSN'er efter 2011, der ikke er formateret som ni på hinanden følgende cifre (ddddddddddd)</span><span class="sxs-lookup"><span data-stu-id="0233d-118">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="0233d-119">**[Kontrolsum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nej, der er ingen Kontrolsum</span><span class="sxs-lookup"><span data-stu-id="0233d-119">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="0233d-120">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** En DLP-politik er 85 % sikker på, at den har registreret denne type følsomme oplysninger, hvis der ligger 300 tegn i nærheden af 300 tegn:</span><span class="sxs-lookup"><span data-stu-id="0233d-120">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="0233d-121">[Funktionen Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finder indhold, der svarer til mønsteret.</span><span class="sxs-lookup"><span data-stu-id="0233d-121">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="0233d-122">Der findes et nøgleord fra [Keyword_ssn.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn)</span><span class="sxs-lookup"><span data-stu-id="0233d-122">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="0233d-123">Eksempler på nøgleord omfatter: *Social Security, Social Security#, Soc Sec , SSN* .</span><span class="sxs-lookup"><span data-stu-id="0233d-123">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="0233d-124">Følgende eksempel udløser f.eks. **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="0233d-124">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="0233d-125">Du kan finde flere oplysninger om, hvad der kræves, for at SSN'er kan registreres for dit indhold, i følgende afsnit i denne artikel: [Hvad søger følsomme informationstyper efter SSN'er](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="0233d-125">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="0233d-126">Brug en anden indbygget type følsomme oplysninger finder du i følgende artikel for at få oplysninger om, hvad der kræves for andre typer: [Hvad de følsomme informationstyper søger efter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="0233d-126">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  