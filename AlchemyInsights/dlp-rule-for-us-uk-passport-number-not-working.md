---
title: DLP-regel for PASNUMMER MELLEM USA og STORBRITANNIEN fungerer ikke
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c63e814059c897531109aa78725e9811b311fb27
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931256"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="c90e1-102">Problemer med DLP - PASnumre i USA/STORBRITANNIEN</span><span class="sxs-lookup"><span data-stu-id="c90e1-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="c90e1-103">**Vigtigt**: Mange SharePoint Online- og OneDrive-kunder kører forretningskritiske programmer mod den tjeneste, der kører i baggrunden.</span><span class="sxs-lookup"><span data-stu-id="c90e1-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="c90e1-104">Disse omfatter indholdsmigrering, Forebyggelse af datatab (DLP) og sikkerhedskopieringsløsninger.</span><span class="sxs-lookup"><span data-stu-id="c90e1-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="c90e1-105">I disse hidtil usete tider tager vi skridt til at sikre, at SharePoint Online- og OneDrive-tjenester forbliver meget tilgængelige og pålidelige for dine brugere, der er afhængige af tjenesten mere end nogensinde før i scenarier for fjernarbejde.</span><span class="sxs-lookup"><span data-stu-id="c90e1-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="c90e1-106">Til støtte for dette mål har vi implementeret strammere begrænsningsgrænser for baggrundsapps (migrering, DLP og backupløsninger) i dagtimerne på hverdage.</span><span class="sxs-lookup"><span data-stu-id="c90e1-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="c90e1-107">Du bør forvente, at disse apps vil opnå meget begrænset gennemløb i disse tider.</span><span class="sxs-lookup"><span data-stu-id="c90e1-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="c90e1-108">I løbet af aftenen og i weekenden for regionen vil tjenesten dog være klar til at behandle en betydeligt større mængde anmodninger fra baggrundsapps.</span><span class="sxs-lookup"><span data-stu-id="c90e1-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="c90e1-109">**DLP problemer med USA / UK pasnumre**</span><span class="sxs-lookup"><span data-stu-id="c90e1-109">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="c90e1-110">Har du problemer med **Forebyggelse af datatab (DLP),** der ikke fungerer for indhold, der indeholder et **amerikansk/britisk pasnummer,** når du bruger en DLP-følsom informationstype i O365?</span><span class="sxs-lookup"><span data-stu-id="c90e1-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="c90e1-111">Hvis det er tilfældet, skal du sørge for, at indholdet indeholder de nødvendige oplysninger om, hvad DLP-politikken søger efter, når den evalueres.</span><span class="sxs-lookup"><span data-stu-id="c90e1-111">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="c90e1-112">For en **pasnummerpolitik** mellem USA og Storbritannien, der er konfigureret med et konfidensniveau på 75 %, evalueres følgende f.eks.</span><span class="sxs-lookup"><span data-stu-id="c90e1-112">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="c90e1-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Ni cifre</span><span class="sxs-lookup"><span data-stu-id="c90e1-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="c90e1-114">**[Mønster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Ni cifre i træk</span><span class="sxs-lookup"><span data-stu-id="c90e1-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="c90e1-115">**[Kontrolsum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nej, der er ingen Kontrolsum</span><span class="sxs-lookup"><span data-stu-id="c90e1-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="c90e1-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** En DLP-politik er 75 % sikker på, at den har registreret denne type følsomme oplysninger, hvis der ligger 300 tegn i nærheden af 300 tegn:</span><span class="sxs-lookup"><span data-stu-id="c90e1-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="c90e1-117">Funktionen Func_usa_uk_passport finder indhold, der svarer til mønsteret.</span><span class="sxs-lookup"><span data-stu-id="c90e1-117">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="c90e1-118">Der findes et nøgleord fra Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="c90e1-118">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="c90e1-119">Følgende eksempel udløser f.eks. **US/UK passport number**</span><span class="sxs-lookup"><span data-stu-id="c90e1-119">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="c90e1-120">Du kan finde flere oplysninger om, hvad der kræves, for at der kan registreres et PASSPORT-nummer mellem USA og Storbritannien for dit indhold, i følgende afsnit i denne artikel: [Hvad søger følsomme informationstyper efter passport-nummer](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number) mellem USA og Storbritannien</span><span class="sxs-lookup"><span data-stu-id="c90e1-120">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="c90e1-121">Brug en anden indbygget type følsomme oplysninger finder du i følgende artikel for at få oplysninger om, hvad der kræves for andre typer: [Hvad de følsomme informationstyper søger efter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="c90e1-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  