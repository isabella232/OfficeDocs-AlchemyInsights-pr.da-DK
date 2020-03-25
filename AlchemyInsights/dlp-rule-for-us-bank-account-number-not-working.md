---
title: DLP-regel for amerikansk bankkontonummer fungerer ikke
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 0b5c1fb175275028c56e47080708520fe115fb38
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932519"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="73017-102">DLP problemer med amerikanske bankkontonumre</span><span class="sxs-lookup"><span data-stu-id="73017-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="73017-103">**Vigtigt**: Mange SharePoint Online- og OneDrive-kunder kører forretningskritiske programmer mod den tjeneste, der kører i baggrunden.</span><span class="sxs-lookup"><span data-stu-id="73017-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="73017-104">Disse omfatter indholdsmigrering, Forebyggelse af datatab (DLP) og sikkerhedskopieringsløsninger.</span><span class="sxs-lookup"><span data-stu-id="73017-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="73017-105">I disse hidtil usete tider tager vi skridt til at sikre, at SharePoint Online- og OneDrive-tjenester forbliver meget tilgængelige og pålidelige for dine brugere, der er afhængige af tjenesten mere end nogensinde før i scenarier for fjernarbejde.</span><span class="sxs-lookup"><span data-stu-id="73017-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="73017-106">Til støtte for dette mål har vi implementeret strammere begrænsningsgrænser for baggrundsapps (migrering, DLP og backupløsninger) i dagtimerne på hverdage.</span><span class="sxs-lookup"><span data-stu-id="73017-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="73017-107">Du bør forvente, at disse apps vil opnå meget begrænset gennemløb i disse tider.</span><span class="sxs-lookup"><span data-stu-id="73017-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="73017-108">I løbet af aftenen og i weekenden for regionen vil tjenesten dog være klar til at behandle en betydeligt større mængde anmodninger fra baggrundsapps.</span><span class="sxs-lookup"><span data-stu-id="73017-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="73017-109">**DLP problemer med amerikanske bankkontonumre**</span><span class="sxs-lookup"><span data-stu-id="73017-109">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="73017-110">Har du problemer med **Forebyggelse af datatab (DLP),** der ikke fungerer for indhold, der indeholder et **amerikansk bankkontonummer,** når du bruger en DLP-følsom informationstype i O365?</span><span class="sxs-lookup"><span data-stu-id="73017-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="73017-111">Hvis det er tilfældet, skal du sørge for, at indholdet indeholder de nødvendige oplysninger om, hvad DLP-politikken søger efter, når den evalueres.</span><span class="sxs-lookup"><span data-stu-id="73017-111">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="73017-112">For en **amerikansk bankkontonummerspolitik,** der er konfigureret med et konfidensniveau på 85 %, evalueres følgende f.eks., for at reglen udløses:</span><span class="sxs-lookup"><span data-stu-id="73017-112">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="73017-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 cifre</span><span class="sxs-lookup"><span data-stu-id="73017-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="73017-114">**[Mønster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 cifre i træk.</span><span class="sxs-lookup"><span data-stu-id="73017-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="73017-115">**[Kontrolsum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nej, der er ingen Kontrolsum</span><span class="sxs-lookup"><span data-stu-id="73017-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="73017-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** En DLP-politik er 75 % sikker på, at den har registreret denne type følsomme oplysninger, hvis der ligger 300 tegn i nærheden af 300 tegn:</span><span class="sxs-lookup"><span data-stu-id="73017-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="73017-117">Det regulære udtryk Regex_usa_bank_account_number finder indhold, der svarer til mønsteret</span><span class="sxs-lookup"><span data-stu-id="73017-117">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="73017-118">Der findes et nøgleord fra Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="73017-118">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="73017-119">Følgende eksempel udløser f.eks. **US Bank Account Number**</span><span class="sxs-lookup"><span data-stu-id="73017-119">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="73017-120">Du kan finde flere oplysninger om, hvad der kræves, for at der kan registreres et **amerikansk bankkontonummer** for dit indhold, i følgende afsnit i denne artikel: [Hvad de følsomme informationstyper søger efter amerikansk bankkontonummer](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="73017-120">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="73017-121">Brug en anden indbygget type følsomme oplysninger finder du i følgende artikel for at få oplysninger om, hvad der kræves for andre typer: [Hvad de følsomme informationstyper søger efter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="73017-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  