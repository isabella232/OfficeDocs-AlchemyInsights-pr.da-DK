---
title: Moderne websted som rodwebsted
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 2e2bb02b9dbaf7f8ede0b4c5ba8c8f29453309cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054696"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="b5e68-102">Moderne websted som rodwebsted</span><span class="sxs-lookup"><span data-stu-id="b5e68-102">Modern site as root site</span></span>

<span data-ttu-id="b5e68-103">Vi er begyndt at udrulning en ny funktion, der vil give dig mulighed for at [bytte din klassiske site root site med en moderne hjemmeside](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="b5e68-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="b5e68-104">Brug [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) til at bytte placeringen af et websted med et andet websted, mens du arkiverer det oprindelige websted.</span><span class="sxs-lookup"><span data-stu-id="b5e68-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="b5e68-105">Tilgængelig for både team websted (ikke forbundet til en gruppe) og kommunikationswebsted.</span><span class="sxs-lookup"><span data-stu-id="b5e68-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="b5e68-106">Du må ikke slette dit klassiske rodwebsted for at oprette et moderne kommunikationswebsted.</span><span class="sxs-lookup"><span data-stu-id="b5e68-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="b5e68-107">Dette understøttes ikke af Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b5e68-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="b5e68-108">Hvis du sletter rodwebstedet, bliver alle SharePoint-websteder i organisationen utilgængelige for alle brugere, indtil du gendanner webstedet eller opretter et nyt websted på samme webadresse.</span><span class="sxs-lookup"><span data-stu-id="b5e68-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="b5e68-109">Vi kommunikerer denne funktion via meddelelsescenteret.</span><span class="sxs-lookup"><span data-stu-id="b5e68-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="b5e68-110">Du kan forvente, at funktionen er aktiveret i din lejer inden længe.</span><span class="sxs-lookup"><span data-stu-id="b5e68-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="b5e68-111">Kendte problemer med swapping sites</span><span class="sxs-lookup"><span data-stu-id="b5e68-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="b5e68-112">Destinationswebstedet kan returnere fejlen "ikke fundet" (HTTP 404) i en kort periode.</span><span class="sxs-lookup"><span data-stu-id="b5e68-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="b5e68-113">Indholdet skal sættes i igen for at opdatere søgeindekset.</span><span class="sxs-lookup"><span data-stu-id="b5e68-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="b5e68-114">Der er ingen manuelle trin kræves her, dette vil ske automatisk.</span><span class="sxs-lookup"><span data-stu-id="b5e68-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="b5e68-115">Alt, hvad der er afhængigt af "statiske" links (f. eks. filsynkronisering og OneNote-filer), skal korrigeres manuelt.</span><span class="sxs-lookup"><span data-stu-id="b5e68-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="b5e68-116">Project Server-websteder skal muligvis valideres for at sikre, at de stadig er tilknyttet korrekt.</span><span class="sxs-lookup"><span data-stu-id="b5e68-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
