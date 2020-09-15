---
title: Moderne websted som rodwebstedet
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666864"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="2ba21-102">Moderne websted som rodwebstedet</span><span class="sxs-lookup"><span data-stu-id="2ba21-102">Modern site as root site</span></span>

<span data-ttu-id="2ba21-103">Vi er gået i kontakt med en ny funktion, der giver dig mulighed for at [udskifte dit klassiske websted med et moderne websted](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="2ba21-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="2ba21-104">Brug [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) for at udskifte placeringen af et websted med et andet websted, mens du arkiverer det oprindelige websted.</span><span class="sxs-lookup"><span data-stu-id="2ba21-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="2ba21-105">Tilgængelig for begge team websteder (ikke forbundet til en gruppe) og kommunikationswebsted.</span><span class="sxs-lookup"><span data-stu-id="2ba21-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="2ba21-106">Slet ikke dit klassiske websted for at oprette et moderne kommunikationswebsted.</span><span class="sxs-lookup"><span data-stu-id="2ba21-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="2ba21-107">Dette understøttes ikke af Microsoft.</span><span class="sxs-lookup"><span data-stu-id="2ba21-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="2ba21-108">Hvis du sletter rodwebstedet, bliver alle SharePoint-websteder i organisationen utilgængelige for alle brugere, indtil du gendanner webstedet eller opretter et nyt websted på den samme URL-adresse.</span><span class="sxs-lookup"><span data-stu-id="2ba21-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="2ba21-109">Vi kommunikerer denne funktion via meddelelses Center.</span><span class="sxs-lookup"><span data-stu-id="2ba21-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="2ba21-110">Du skal forvente, at funktionen skulle slås til på din lejer i sin tid.</span><span class="sxs-lookup"><span data-stu-id="2ba21-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="2ba21-111">Kendte problemer med swap websteder</span><span class="sxs-lookup"><span data-stu-id="2ba21-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="2ba21-112">Destinationswebstedet kan returnere fejlen "ikke fundet" (HTTP 404) for en kort periode.</span><span class="sxs-lookup"><span data-stu-id="2ba21-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="2ba21-113">Indhold skal gennemsøges for at opdatere søgeindekset.</span><span class="sxs-lookup"><span data-stu-id="2ba21-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="2ba21-114">Der kræves intet manuelt trin her, det sker automatisk.</span><span class="sxs-lookup"><span data-stu-id="2ba21-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="2ba21-115">Alt afhængigt af "statiske" links (f. eks. filsynkronisering og OneNote-filer) skal rettes manuelt.</span><span class="sxs-lookup"><span data-stu-id="2ba21-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="2ba21-116">Project Server-websteder skal muligvis valideres for at sikre, at de stadig er knyttet korrekt.</span><span class="sxs-lookup"><span data-stu-id="2ba21-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
