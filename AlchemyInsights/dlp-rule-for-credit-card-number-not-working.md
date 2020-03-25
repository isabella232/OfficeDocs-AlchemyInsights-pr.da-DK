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
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932437"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="42107-102">DLP problemer med kreditkortnumre</span><span class="sxs-lookup"><span data-stu-id="42107-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="42107-103">**Vigtigt**: Mange SharePoint Online- og OneDrive-kunder kører forretningskritiske programmer mod den tjeneste, der kører i baggrunden.</span><span class="sxs-lookup"><span data-stu-id="42107-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="42107-104">Disse omfatter indholdsmigrering, Forebyggelse af datatab (DLP) og sikkerhedskopieringsløsninger.</span><span class="sxs-lookup"><span data-stu-id="42107-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="42107-105">I disse hidtil usete tider tager vi skridt til at sikre, at SharePoint Online- og OneDrive-tjenester forbliver meget tilgængelige og pålidelige for dine brugere, der er afhængige af tjenesten mere end nogensinde før i scenarier for fjernarbejde.</span><span class="sxs-lookup"><span data-stu-id="42107-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="42107-106">Til støtte for dette mål har vi implementeret strammere begrænsningsgrænser for baggrundsapps (migrering, DLP og backupløsninger) i dagtimerne på hverdage.</span><span class="sxs-lookup"><span data-stu-id="42107-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="42107-107">Du bør forvente, at disse apps vil opnå meget begrænset gennemløb i disse tider.</span><span class="sxs-lookup"><span data-stu-id="42107-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="42107-108">I løbet af aftenen og i weekenden for regionen vil tjenesten dog være klar til at behandle en betydeligt større mængde anmodninger fra baggrundsapps.</span><span class="sxs-lookup"><span data-stu-id="42107-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="42107-109">**DLP problemer med kreditkortnumre**</span><span class="sxs-lookup"><span data-stu-id="42107-109">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="42107-110">Har du problemer med **Forebyggelse af datatab (DLP),** der ikke fungerer for indhold, der indeholder et **kreditkortnummer,** når du bruger en DLP-følsom informationstype i O365?</span><span class="sxs-lookup"><span data-stu-id="42107-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="42107-111">Hvis det er tilfældet, skal du sørge for, at indholdet indeholder de nødvendige oplysninger for at udløse DLP-politikken, når den evalueres.</span><span class="sxs-lookup"><span data-stu-id="42107-111">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="42107-112">For en **kreditkortpolitik,** der er konfigureret med et konfidensniveau på 85 %, evalueres følgende f.eks., for at reglen udløses:</span><span class="sxs-lookup"><span data-stu-id="42107-112">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="42107-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 cifre, der kan formateres eller uformateret (dddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddd</span><span class="sxs-lookup"><span data-stu-id="42107-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="42107-114">**[Mønster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Meget komplekst og robust mønster, der registrerer kort fra alle større mærker over hele verden, herunder Visa, MasterCard, Discover Card, JCB, American Express, gavekort og spisekort.</span><span class="sxs-lookup"><span data-stu-id="42107-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="42107-115">**[Kontrolsum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Ja, Luhn checksum</span><span class="sxs-lookup"><span data-stu-id="42107-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="42107-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** En DLP-politik er 85 % sikker på, at den har registreret denne type følsomme oplysninger, hvis der ligger 300 tegn i nærheden af 300 tegn:</span><span class="sxs-lookup"><span data-stu-id="42107-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="42107-117">Funktionen Func_credit_card finder indhold, der svarer til mønsteret.</span><span class="sxs-lookup"><span data-stu-id="42107-117">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="42107-118">Et af følgende er sandt:</span><span class="sxs-lookup"><span data-stu-id="42107-118">One of the following is true:</span></span>

  - <span data-ttu-id="42107-119">Der findes et nøgleord fra Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="42107-119">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="42107-120">Der findes et nøgleord fra Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="42107-120">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="42107-121">Funktionen Func_expiration_date finder en dato i det rigtige datoformat.</span><span class="sxs-lookup"><span data-stu-id="42107-121">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="42107-122">Kontrolsummen passerer</span><span class="sxs-lookup"><span data-stu-id="42107-122">The checksum passes</span></span>

    <span data-ttu-id="42107-123">Følgende eksempel udløser f.eks.</span><span class="sxs-lookup"><span data-stu-id="42107-123">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="42107-124">Visum: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="42107-124">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="42107-125">Udløber: 2/2009</span><span class="sxs-lookup"><span data-stu-id="42107-125">Expires: 2/2009</span></span>

<span data-ttu-id="42107-126">Du kan finde flere oplysninger om, hvad der kræves, for at der kan registreres et **kreditkortnummer** for dit indhold, i følgende afsnit i denne artikel: [Hvad søger de følsomme informationstyper efter kreditkort#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="42107-126">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="42107-127">Brug en anden indbygget type følsomme oplysninger finder du i følgende artikel for at få oplysninger om, hvad der kræves for andre typer: [Hvad de følsomme informationstyper søger efter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="42107-127">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  