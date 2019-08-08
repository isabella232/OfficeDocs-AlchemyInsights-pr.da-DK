---
title: Moderne sted som rodwebstedet
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1874"
- "9000265"
ms.openlocfilehash: b30fc3258bb76c0ab4bf10af0ec9317417f7c663
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/07/2019
ms.locfileid: "36232709"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="4d421-102">Moderne sted som rodwebstedet</span><span class="sxs-lookup"><span data-stu-id="4d421-102">Modern site as root site</span></span>

<span data-ttu-id="4d421-103">Vi er begyndt til distribuering af en ny funktion, der gør det muligt at skifte din klassiske websted-rodwebstedet med et moderne websted.</span><span class="sxs-lookup"><span data-stu-id="4d421-103">We have begun to rollout a new feature that will allow you to swap your classic site root site with a modern site.</span></span> <span data-ttu-id="4d421-104">Brug [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) til at skifte placeringen af et websted med et andet websted under arkivering af det oprindelige websted.</span><span class="sxs-lookup"><span data-stu-id="4d421-104">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="4d421-105">Tilgængelig for både Team (ikke har forbindelse til en gruppe) og kommunikation.</span><span class="sxs-lookup"><span data-stu-id="4d421-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

>[!Important]
> <span data-ttu-id="4d421-106">Slet ikke klassiske rod-webstedet for at oprette et websted til et moderne kommunikation.</span><span class="sxs-lookup"><span data-stu-id="4d421-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="4d421-107">Dette understøttes ikke af Microsoft.</span><span class="sxs-lookup"><span data-stu-id="4d421-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="4d421-108">Slette rodwebstedet, bliver alle SharePoint-websteder i din organisation utilgængelige for alle brugere, før du gendanne webstedet eller oprette et nyt websted med samme URL-adresse.</span><span class="sxs-lookup"><span data-stu-id="4d421-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="4d421-109">Vi kommunikere denne funktion via Beskedcentret.</span><span class="sxs-lookup"><span data-stu-id="4d421-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="4d421-110">Du kan forvente, at funktionen være aktiveret i din lejer kort.</span><span class="sxs-lookup"><span data-stu-id="4d421-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="4d421-111">Kendte problemer i forbindelse med udskiftning af websteder</span><span class="sxs-lookup"><span data-stu-id="4d421-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="4d421-112">Målwebstedet kan returnere fejlen "ikke fundet" (HTTP 404) for en kort periode.</span><span class="sxs-lookup"><span data-stu-id="4d421-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="4d421-113">Indholdet skal være recrawled for at opdatere søgeindekset.</span><span class="sxs-lookup"><span data-stu-id="4d421-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="4d421-114">Der er ingen manuelle trin, der kræves her, dette gøres automatisk.</span><span class="sxs-lookup"><span data-stu-id="4d421-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="4d421-115">Alt afhængig af "statiske" links (f.eks filsynkronisering og OneNote-filer) skal rettes manuelt.</span><span class="sxs-lookup"><span data-stu-id="4d421-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="4d421-116">Project Server-websteder skal valideres for at sikre, at de er stadig knyttet korrekt.</span><span class="sxs-lookup"><span data-stu-id="4d421-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
