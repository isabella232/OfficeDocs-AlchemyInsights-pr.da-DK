---
title: Byt dit klassiske rodwebsted med et moderne websted
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
ms.openlocfilehash: bd477d90ab7e6737aafffc57d931aad2bd0351e8
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/04/2019
ms.locfileid: "36749254"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="42143-102">Byt dit klassiske rodwebsted med et moderne websted</span><span class="sxs-lookup"><span data-stu-id="42143-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="42143-103">Hvis dit miljø blev oprettet før april 2019, kan du ændre rodwebstedet til et moderne websted ved hjælp af Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="42143-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="42143-104">Hvis du har et andet websted, som du vil bruge som rodwebsted, kan du erstatte [(bytte) rodwebstedet](https://docs.microsoft.com/sharepoint/modern-root-site) med det.</span><span class="sxs-lookup"><span data-stu-id="42143-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="42143-105">Brug [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) til at bytte placeringen af et websted med et andet websted, mens du arkiverer det oprindelige websted.</span><span class="sxs-lookup"><span data-stu-id="42143-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="42143-106">Tilgængelig for både team websted (ikke forbundet til en gruppe) og kommunikationswebsted.</span><span class="sxs-lookup"><span data-stu-id="42143-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="42143-107">Yderligere funktioner vil blive indført snart, der vil give dig mulighed for at fortsætte med at bruge indholdet på webstedet, men konvertere det eksisterende websted til en kommunikation site.</span><span class="sxs-lookup"><span data-stu-id="42143-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="42143-108">Disse funktioner vil blive rullet ud gradvist.</span><span class="sxs-lookup"><span data-stu-id="42143-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="42143-109">Fortsæt med at kontrollere Office 365 Message Center for opdateringer.</span><span class="sxs-lookup"><span data-stu-id="42143-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="42143-110">Kendte problemer med swapping sites</span><span class="sxs-lookup"><span data-stu-id="42143-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="42143-111">Destinationswebstedet kan returnere fejlen "ikke fundet" (HTTP 404) i en kort periode.</span><span class="sxs-lookup"><span data-stu-id="42143-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="42143-112">Indholdet skal sættes i igen for at opdatere søgeindekset.</span><span class="sxs-lookup"><span data-stu-id="42143-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="42143-113">Der er ingen manuelle trin påkrævet-dette vil ske automatisk.</span><span class="sxs-lookup"><span data-stu-id="42143-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="42143-114">Alt, hvad der er afhængigt af "statiske" links (f. eks. filsynkronisering og OneNote-filer), skal korrigeres manuelt.</span><span class="sxs-lookup"><span data-stu-id="42143-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="42143-115">Hvis kildewebstedet var et organisations nyhedswebsted, bør du opdatere URL-adressen.</span><span class="sxs-lookup"><span data-stu-id="42143-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="42143-116">Få en liste over alle organisatoriske nyhedssites.</span><span class="sxs-lookup"><span data-stu-id="42143-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="42143-117">Project Server-websteder skal muligvis valideres for at sikre, at de stadig er tilknyttet korrekt.</span><span class="sxs-lookup"><span data-stu-id="42143-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





