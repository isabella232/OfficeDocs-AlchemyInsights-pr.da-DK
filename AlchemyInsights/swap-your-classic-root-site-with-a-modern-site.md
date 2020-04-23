---
title: Byt din Klassiske rod site med en moderne site
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: f4831c6a232a4dee0f8f5ac0c83e4307221cfe2d
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741538"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="1e11b-102">Byt din Klassiske rod site med en moderne site</span><span class="sxs-lookup"><span data-stu-id="1e11b-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="1e11b-103">Hvis dit miljø blev konfigureret før april 2019, kan du ændre rodwebstedet til et moderne websted ved hjælp af Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="1e11b-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="1e11b-104">Hvis du har et andet websted, som du vil bruge som rodwebsted, kan du erstatte [(bytte) rodwebstedet](https://docs.microsoft.com/sharepoint/modern-root-site) med det.</span><span class="sxs-lookup"><span data-stu-id="1e11b-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="1e11b-105">Brug [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) til at bytte placeringen af et websted med et andet websted, mens du arkiverer det oprindelige websted.</span><span class="sxs-lookup"><span data-stu-id="1e11b-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="1e11b-106">Tilgængelig for både teamwebsted (ikke forbundet til en gruppe) og kommunikationswebsted.</span><span class="sxs-lookup"><span data-stu-id="1e11b-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="1e11b-107">Yderligere funktioner vil blive indført snart, som vil give dig mulighed for at fortsætte med at bruge indholdet på webstedet, men konvertere det eksisterende websted til en kommunikation site.</span><span class="sxs-lookup"><span data-stu-id="1e11b-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="1e11b-108">Disse funktioner vil blive udrullet gradvist.</span><span class="sxs-lookup"><span data-stu-id="1e11b-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="1e11b-109">Fortsæt med at kontrollere opdateringerne i Meddelelsescenter.</span><span class="sxs-lookup"><span data-stu-id="1e11b-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="1e11b-110">Kendte problemer med byttewebsteder</span><span class="sxs-lookup"><span data-stu-id="1e11b-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="1e11b-111">Destinationswebstedet kan returnere en "ikke fundet" (HTTP 404) fejl i en kort periode.</span><span class="sxs-lookup"><span data-stu-id="1e11b-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="1e11b-112">Indholdet skal crawles igen for at opdatere søgeindekset.</span><span class="sxs-lookup"><span data-stu-id="1e11b-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="1e11b-113">Der er ingen manuel trin påkrævet - dette vil ske automatisk.</span><span class="sxs-lookup"><span data-stu-id="1e11b-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="1e11b-114">Alt, hvad der er afhængigt af "statiske" links (f.eks. filsynkronisering og OneNote-filer), skal rettes manuelt.</span><span class="sxs-lookup"><span data-stu-id="1e11b-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="1e11b-115">Hvis kildewebstedet var et organisationsnyhedswebsted, skal du opdatere URL-adressen.</span><span class="sxs-lookup"><span data-stu-id="1e11b-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="1e11b-116">Få en liste over alle organisatoriske nyhedssites.</span><span class="sxs-lookup"><span data-stu-id="1e11b-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="1e11b-117">Project Server-websteder skal muligvis valideres for at sikre, at de stadig er tilknyttet korrekt.</span><span class="sxs-lookup"><span data-stu-id="1e11b-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
