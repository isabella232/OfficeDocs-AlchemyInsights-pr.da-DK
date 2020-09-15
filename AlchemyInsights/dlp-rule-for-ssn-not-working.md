---
title: DLP-regel for CPR virker ikke
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
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679363"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="a0ce7-102">DLP-problemer med sociale sikkerheds numre</span><span class="sxs-lookup"><span data-stu-id="a0ce7-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="a0ce7-103">**Vigtigt**: I disse hidtil usete tider bestræber vi os på at sikre, at SharePoint Online- og OneDrive-tjenesterne fastholder sin høje tilgængelighed. Hvis du ønsker flere oplysninger, skal du besøge [Midlertidige funktionsjusteringer i SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="a0ce7-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="a0ce7-104">**DLP-problemer med CPR**</span><span class="sxs-lookup"><span data-stu-id="a0ce7-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="a0ce7-105">Har du problemer med forebyggelse af datatab **(DLP)** , fungerer det ikke for indhold, der indeholder et **CPR-nummer (CPR)** , når du bruger en følsom oplysningstype i Microsoft 365?</span><span class="sxs-lookup"><span data-stu-id="a0ce7-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="a0ce7-106">Hvis det er tilfældet, skal du sørge for, at dit indhold indeholder de nødvendige oplysninger om, hvad DLP-politikken ser ud.</span><span class="sxs-lookup"><span data-stu-id="a0ce7-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="a0ce7-107">For en CPR-politik, der er konfigureret med et tillidsniveau på 85%, evalueres følgende og skal registreres, for at reglen udløses:</span><span class="sxs-lookup"><span data-stu-id="a0ce7-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="a0ce7-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 cifre, som kan være i et formateret eller ikke-formateret mønster</span><span class="sxs-lookup"><span data-stu-id="a0ce7-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="a0ce7-109">**[Mønster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Fire funktioner ser ud efter CPR i fire forskellige mønstre:</span><span class="sxs-lookup"><span data-stu-id="a0ce7-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="a0ce7-110">Func_ssn finder CPR med en stærk formatering før 2011, der er formateret med bindestreger eller mellemrum (DDD-DD-dddd eller DDD DD dddd)</span><span class="sxs-lookup"><span data-stu-id="a0ce7-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="a0ce7-111">Func_unformatted_ssn finder CPR 2011 med en stærk formatering, der er formateret som ni fortløbende cifre (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="a0ce7-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="a0ce7-112">Func_randomized_formatted_ssn finder post-2011 CPR, der er formateret med bindestreger eller mellemrum (DDD-DD-dddd eller DDD DD dddd)</span><span class="sxs-lookup"><span data-stu-id="a0ce7-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="a0ce7-113">Func_randomized_unformatted_ssn finder post-2011 CPR, der er uformateret som ni fortløbende cifre (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="a0ce7-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="a0ce7-114">**[Kontrolsum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Nej, der er ingen kontrolsum</span><span class="sxs-lookup"><span data-stu-id="a0ce7-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="a0ce7-115">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** En DLP-politik er 85% sikker på, at den har registreret denne type af følsomme oplysninger, hvis det inden for en afstand af 300 tegn:</span><span class="sxs-lookup"><span data-stu-id="a0ce7-115">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="a0ce7-116">[Funktionen Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finder indhold, der svarer til mønsteret.</span><span class="sxs-lookup"><span data-stu-id="a0ce7-116">The [function Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="a0ce7-117">Der er fundet et nøgleord fra [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) .</span><span class="sxs-lookup"><span data-stu-id="a0ce7-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) is found.</span></span> <span data-ttu-id="a0ce7-118">Eksempler på nøgleord omfatter:  *social sikring, social sikrings nummer, soc SEC, CPR*  .</span><span class="sxs-lookup"><span data-stu-id="a0ce7-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="a0ce7-119">Eksempelvis vil følgende eksempel udløse for DLP CPR-politikken: **CPR: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="a0ce7-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="a0ce7-120">Du kan finde flere oplysninger om, hvad der kræves for CPR til dit indhold, i følgende afsnit i denne artikel: [hvad de følsomme oplysningstyper ser ud efter CPR](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="a0ce7-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="a0ce7-121">Ved hjælp af en anden indbygget type af følsomme oplysninger, skal du se følgende artikel for oplysninger om, hvad der kræves til andre typer: [hvad de følsomme oplysningstyper ser ud for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="a0ce7-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  