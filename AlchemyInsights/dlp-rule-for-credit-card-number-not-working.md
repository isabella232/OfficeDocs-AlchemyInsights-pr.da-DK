---
title: DLP-regel for kreditkortnummer fungerer ikke
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 40a4a1668039b70455e09ee662359c05235645e8
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977192"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="2877f-102">DLP problemer med kreditkortnumre</span><span class="sxs-lookup"><span data-stu-id="2877f-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="2877f-103">**Vigtigt:** I disse hidtil usete tider tager vi skridt til at sikre, at SharePoint Online- og OneDrive-tjenester forbliver meget tilgængelige – Besøg [midlertidige sharepoint onlinefunktionsjusteringer](https://aka.ms/ODSPAdjustments) for at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="2877f-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="2877f-104">**DLP problemer med kreditkortnumre**</span><span class="sxs-lookup"><span data-stu-id="2877f-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="2877f-105">Har du problemer med **Forebyggelse af datatab (DLP),** der ikke fungerer for indhold, der indeholder et **kreditkortnummer,** når du bruger en DLP-følsom informationstype i O365?</span><span class="sxs-lookup"><span data-stu-id="2877f-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="2877f-106">Hvis det er tilfældet, skal du sørge for, at indholdet indeholder de nødvendige oplysninger for at udløse DLP-politikken, når den evalueres.</span><span class="sxs-lookup"><span data-stu-id="2877f-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="2877f-107">For en **kreditkortpolitik,** der er konfigureret med et konfidensniveau på 85 %, evalueres følgende f.eks., for at reglen udløses:</span><span class="sxs-lookup"><span data-stu-id="2877f-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="2877f-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 cifre, der kan formateres eller uformateret (dddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddd</span><span class="sxs-lookup"><span data-stu-id="2877f-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="2877f-109">**[Mønster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Meget komplekst og robust mønster, der registrerer kort fra alle større mærker over hele verden, herunder Visa, MasterCard, Discover Card, JCB, American Express, gavekort og spisekort.</span><span class="sxs-lookup"><span data-stu-id="2877f-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="2877f-110">**[Kontrolsum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Ja, Luhn checksum</span><span class="sxs-lookup"><span data-stu-id="2877f-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="2877f-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** En DLP-politik er 85 % sikker på, at den har registreret denne type følsomme oplysninger, hvis der ligger 300 tegn i nærheden af 300 tegn:</span><span class="sxs-lookup"><span data-stu-id="2877f-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="2877f-112">Funktionen Func_credit_card finder indhold, der svarer til mønsteret.</span><span class="sxs-lookup"><span data-stu-id="2877f-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="2877f-113">Et af følgende er sandt:</span><span class="sxs-lookup"><span data-stu-id="2877f-113">One of the following is true:</span></span>

  - <span data-ttu-id="2877f-114">Der findes et nøgleord fra Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="2877f-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="2877f-115">Der findes et nøgleord fra Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="2877f-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="2877f-116">Funktionen Func_expiration_date finder en dato i det rigtige datoformat.</span><span class="sxs-lookup"><span data-stu-id="2877f-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="2877f-117">Kontrolsummen passerer</span><span class="sxs-lookup"><span data-stu-id="2877f-117">The checksum passes</span></span>

    <span data-ttu-id="2877f-118">Følgende eksempel udløser f.eks.</span><span class="sxs-lookup"><span data-stu-id="2877f-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="2877f-119">Visum: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="2877f-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="2877f-120">Udløber: 2/2009</span><span class="sxs-lookup"><span data-stu-id="2877f-120">Expires: 2/2009</span></span>

<span data-ttu-id="2877f-121">Du kan finde flere oplysninger om, hvad der kræves, for at der kan registreres et **kreditkortnummer** for dit indhold, i følgende afsnit i denne artikel: [Hvad søger de følsomme informationstyper efter kreditkort#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="2877f-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="2877f-122">Brug en anden indbygget type følsomme oplysninger finder du i følgende artikel for at få oplysninger om, hvad der kræves for andre typer: [Hvad de følsomme informationstyper søger efter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="2877f-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  