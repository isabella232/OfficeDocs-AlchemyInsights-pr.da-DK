---
title: Byt dine Classic-rodwebstedet med et moderne websted
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 0f6f962314d9099bd21c281a23ad2e95742da4a8
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270738"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="d162f-102">Byt dine Classic-rodwebstedet med et moderne websted</span><span class="sxs-lookup"><span data-stu-id="d162f-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="d162f-103">Hvis dit miljø blev oprettet før April 2019, kan du ændre rod-websted til et moderne websted ved hjælp af Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="d162f-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="d162f-104">Hvis du har et andet websted, som du vil bruge som rod-websted, kan du erstatte (swapfilen) rod-websted med den.</span><span class="sxs-lookup"><span data-stu-id="d162f-104">If you have a different site that you want to use as your root site, you can replace (swap) the root site with it.</span></span> 
    - <span data-ttu-id="d162f-105">Brug [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) til at skifte placeringen af et websted med et andet websted under arkivering af det oprindelige websted.</span><span class="sxs-lookup"><span data-stu-id="d162f-105">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="d162f-106">Tilgængelig for både Team (ikke har forbindelse til en gruppe) og kommunikation.</span><span class="sxs-lookup"><span data-stu-id="d162f-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="d162f-107">Ekstra funktioner introduceres snarest, der giver dig mulighed at holde med indhold på webstedet, men konvertere det eksisterende websted til et kommunikationswebsted.</span><span class="sxs-lookup"><span data-stu-id="d162f-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="d162f-108">Disse funktioner vil blive gennemført gradvist.</span><span class="sxs-lookup"><span data-stu-id="d162f-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="d162f-109">Fortsætte med at kontrollere Office 365 Message Center for opdateringer.</span><span class="sxs-lookup"><span data-stu-id="d162f-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="d162f-110">Kendte problemer i forbindelse med udskiftning af websteder</span><span class="sxs-lookup"><span data-stu-id="d162f-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="d162f-111">Målwebstedet kan returnere fejlen "ikke fundet" (HTTP 404) for en kort periode.</span><span class="sxs-lookup"><span data-stu-id="d162f-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="d162f-112">Indholdet skal være recrawled for at opdatere søgeindekset.</span><span class="sxs-lookup"><span data-stu-id="d162f-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="d162f-113">Der er ingen manuelle trin, der kræves - dette gøres automatisk.</span><span class="sxs-lookup"><span data-stu-id="d162f-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="d162f-114">Alt afhængig af "statiske" links (f.eks filsynkronisering og OneNote-filer) skal rettes manuelt.</span><span class="sxs-lookup"><span data-stu-id="d162f-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="d162f-115">Hvis kildewebstedet var en organisatorisk nyhedswebsted, kan du opdatere URL-adressen.</span><span class="sxs-lookup"><span data-stu-id="d162f-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="d162f-116">Få en liste over websteder med alle Nyheder i virksomheden.</span><span class="sxs-lookup"><span data-stu-id="d162f-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="d162f-117">Project Server-websteder skal valideres for at sikre, at de er stadig knyttet korrekt.</span><span class="sxs-lookup"><span data-stu-id="d162f-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





