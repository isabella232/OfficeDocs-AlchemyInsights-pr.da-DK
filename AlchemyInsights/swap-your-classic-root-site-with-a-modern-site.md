---
title: Ombyt dit klassiske rod-websted med et moderne websted
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691173"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="bc77f-102">Ombyt dit klassiske rod-websted med et moderne websted</span><span class="sxs-lookup"><span data-stu-id="bc77f-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="bc77f-103">Hvis dit miljø er konfigureret før april 2019, kan du ændre rodwebstedet til et moderne websted ved hjælp af Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="bc77f-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="bc77f-104">Hvis du har et andet websted, som du vil bruge som dit rodwebsted, kan du erstatte [(bytte) om på rodwebstedet](https://docs.microsoft.com/sharepoint/modern-root-site) .</span><span class="sxs-lookup"><span data-stu-id="bc77f-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="bc77f-105">Brug [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) for at udskifte placeringen af et websted med et andet websted, mens du arkiverer det oprindelige websted.</span><span class="sxs-lookup"><span data-stu-id="bc77f-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="bc77f-106">Tilgængelig for begge team websteder (ikke forbundet til en gruppe) og kommunikationswebsted.</span><span class="sxs-lookup"><span data-stu-id="bc77f-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="bc77f-107">Der vil blive introduceret flere muligheder, der giver dig mulighed for at fortsætte med at bruge indholdet på webstedet, men konvertere det eksisterende websted til et kommunikationswebsted.</span><span class="sxs-lookup"><span data-stu-id="bc77f-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="bc77f-108">Disse egenskaber bliver udrullet gradvist.</span><span class="sxs-lookup"><span data-stu-id="bc77f-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="bc77f-109">Fortsæt med at kontrollere meddelelses Center for opdateringer.</span><span class="sxs-lookup"><span data-stu-id="bc77f-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="bc77f-110">Kendte problemer med swap websteder</span><span class="sxs-lookup"><span data-stu-id="bc77f-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="bc77f-111">Destinationswebstedet kan returnere fejlen "ikke fundet" (HTTP 404) for en kort periode.</span><span class="sxs-lookup"><span data-stu-id="bc77f-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="bc77f-112">Indhold skal gennemsøges for at opdatere søgeindekset.</span><span class="sxs-lookup"><span data-stu-id="bc77f-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="bc77f-113">Der kræves intet manuelt trin. dette sker automatisk.</span><span class="sxs-lookup"><span data-stu-id="bc77f-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="bc77f-114">Alt afhængigt af "statiske" links (f. eks. filsynkronisering og OneNote-filer) skal rettes manuelt.</span><span class="sxs-lookup"><span data-stu-id="bc77f-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="bc77f-115">Hvis kildewebstedet var et organisations nyhedswebsted, skal du opdatere URL-adressen.</span><span class="sxs-lookup"><span data-stu-id="bc77f-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="bc77f-116">Få en liste over alle organisationens nyheds websteder.</span><span class="sxs-lookup"><span data-stu-id="bc77f-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="bc77f-117">Project Server-websteder skal muligvis valideres for at sikre, at de stadig er knyttet korrekt.</span><span class="sxs-lookup"><span data-stu-id="bc77f-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
