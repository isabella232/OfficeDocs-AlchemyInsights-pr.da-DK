---
title: Flere oplysninger om DLP-problemer
ms.author: pebaum
author: pebaum
manager: laurawi
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2447"
- "3200001"
ms.openlocfilehash: 6525cee0555f1ae67b7d4e32445b9a1537d4a804
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932688"
---
# <a name="information-about-dlp-issues"></a><span data-ttu-id="83fbe-102">Oplysninger om DLP-problemer</span><span class="sxs-lookup"><span data-stu-id="83fbe-102">Information about DLP issues</span></span>

<span data-ttu-id="83fbe-103">**Vigtigt**: Mange SharePoint Online- og OneDrive-kunder kører forretningskritiske programmer mod den tjeneste, der kører i baggrunden.</span><span class="sxs-lookup"><span data-stu-id="83fbe-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="83fbe-104">Disse omfatter indholdsmigrering, Forebyggelse af datatab (DLP) og sikkerhedskopieringsløsninger.</span><span class="sxs-lookup"><span data-stu-id="83fbe-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="83fbe-105">I disse hidtil usete tider tager vi skridt til at sikre, at SharePoint Online- og OneDrive-tjenester forbliver meget tilgængelige og pålidelige for dine brugere, der er afhængige af tjenesten mere end nogensinde før i scenarier for fjernarbejde.</span><span class="sxs-lookup"><span data-stu-id="83fbe-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="83fbe-106">Til støtte for dette mål har vi implementeret strammere begrænsningsgrænser for baggrundsapps (migrering, DLP og backupløsninger) i dagtimerne på hverdage.</span><span class="sxs-lookup"><span data-stu-id="83fbe-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="83fbe-107">Du bør forvente, at disse apps vil opnå meget begrænset gennemløb i disse tider.</span><span class="sxs-lookup"><span data-stu-id="83fbe-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="83fbe-108">I løbet af aftenen og i weekenden for regionen vil tjenesten dog være klar til at behandle en betydeligt større mængde anmodninger fra baggrundsapps.</span><span class="sxs-lookup"><span data-stu-id="83fbe-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="83fbe-109">**Oplysninger om DLP-politik**</span><span class="sxs-lookup"><span data-stu-id="83fbe-109">**Information on DLP policy**</span></span>

<span data-ttu-id="83fbe-110">Med en DLP-politik kan du identificere, overvåge og automatisk beskytte følsomme oplysninger på tværs af Office 365.</span><span class="sxs-lookup"><span data-stu-id="83fbe-110">With a DLP policy, you can identify, monitor, and automatically protect sensitive information across Office 365.</span></span>

<span data-ttu-id="83fbe-111">Besøg disse links for mere information:</span><span class="sxs-lookup"><span data-stu-id="83fbe-111">Please visit these links for more information:</span></span>

- [<span data-ttu-id="83fbe-112">Oversigt over forebyggelse af datatab</span><span class="sxs-lookup"><span data-stu-id="83fbe-112">Overview of data loss prevention</span></span>](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies)
- [<span data-ttu-id="83fbe-113">Hvad de følsomme informationstyper søger efter</span><span class="sxs-lookup"><span data-stu-id="83fbe-113">What the sensitive information types look for</span></span>](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
- [<span data-ttu-id="83fbe-114">Oprette en brugerdefineret følsom oplysningstype</span><span class="sxs-lookup"><span data-stu-id="83fbe-114">Create a custom sensitive information type</span></span>](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)
- [<span data-ttu-id="83fbe-115">Send mailmeddelelser, og vis politiktip</span><span class="sxs-lookup"><span data-stu-id="83fbe-115">Send email notifications and show policy tips</span></span>](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)
- [<span data-ttu-id="83fbe-116">Beskytte SharePoint Online-filer med opbevaringsetiketter og DLP</span><span class="sxs-lookup"><span data-stu-id="83fbe-116">Protect SharePoint Online files with retention labels and DLP</span></span>](https://docs.microsoft.com/office365/securitycompliance/protect-sharepoint-online-files-with-office-365-labels-and-dlp)
- [<span data-ttu-id="83fbe-117">DLP og Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="83fbe-117">DLP and Microsoft Teams</span></span>](https://docs.microsoft.com/office365/securitycompliance/dlp-microsoft-teams)

<span data-ttu-id="83fbe-118">Hvis du vil teste dine data med en indbygget eller brugerdefineret følsom oplysningstype, skal du bruge indstillingen **Testtype** under **Klassifikationer** > **Følsomme oplysningstyper**.</span><span class="sxs-lookup"><span data-stu-id="83fbe-118">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="83fbe-119">Yderligere oplysninger finder du i [Test af brugerdefinerede følsomme oplysningstyper](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="83fbe-119">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>