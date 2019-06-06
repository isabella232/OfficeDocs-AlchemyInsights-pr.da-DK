---
title: Administrere ordbøger til søgningen i SharePoint Online
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c2960093bb1cfb649c26528c9f671e6d720ff237
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/05/2019
ms.locfileid: "34736047"
---
# <a name="search-in-sharepoint-online"></a><span data-ttu-id="f136f-102">Søg i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="f136f-102">Search in SharePoint Online</span></span>

<span data-ttu-id="f136f-103">Indholdet skal gennemsøges og tilføjet i søgeindekset for brugerne at finde det, de søger efter, i SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="f136f-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="f136f-104">Indhold gennemsøges automatisk baseret på en foruddefineret gennemsøgning tidsplan (gennemsøgning tidsplanen ikke kan ændres).</span><span class="sxs-lookup"><span data-stu-id="f136f-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="f136f-105">Crawleren henter indhold, der er blevet ændret siden den seneste gennemsøgning og opdaterer indekset.</span><span class="sxs-lookup"><span data-stu-id="f136f-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="f136f-106">Følg nedenstående trin for at sikre indhold gennemsøges og indekset bliver opdateret.</span><span class="sxs-lookup"><span data-stu-id="f136f-106">To ensure content is crawled and the index is updated, follow the steps below.</span></span>

<span data-ttu-id="f136f-107">Kontroller, at indholdet kan findes ved at gøre webstedets indhold kan søges.</span><span class="sxs-lookup"><span data-stu-id="f136f-107">Make sure content can be found by making site content searchable.</span></span> <span data-ttu-id="f136f-108">Yderligere oplysninger finder du i [aktivere indhold på et websted, der skal søges](https://docs.microsoft.com/en-us/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="f136f-108">For more info, see [Enable content on a site to be searchable](https://docs.microsoft.com/en-us/sharepoint/make-site-content-searchable).</span></span>

<span data-ttu-id="f136f-109">Når du har ændret en administreret egenskab, eller når du har ændret tilknytning af gennemsøgt og administrerede skal egenskaber for webstedet være gennemsøgt igen, før ændringerne afspejles i søgeindekset.</span><span class="sxs-lookup"><span data-stu-id="f136f-109">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

<span data-ttu-id="f136f-110">Indeksere webstedet igen, da ændringerne foretages i search-skema, og ikke på webstedet faktiske crawleren ikke automatisk.</span><span class="sxs-lookup"><span data-stu-id="f136f-110">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

<span data-ttu-id="f136f-111">Flere oplysninger, skal du [manuelt anmode om gennemsøgning og indeksering igen af et websted, et bibliotek eller en liste](https://docs.microsoft.com/en-us/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="f136f-111">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/en-us/sharepoint/crawl-site-conten).</span></span>

 <span data-ttu-id="f136f-112">Vent mindst 24 timer efter manuelt anmode om en gennemsøgning og fuld gendanne indekset for at se, hvis du stadig har et problem.</span><span class="sxs-lookup"><span data-stu-id="f136f-112">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

<span data-ttu-id="f136f-113">Hvis der er gået mere end 24 timer, da du startede gennemsøgning og fuld indekseres, skal du logge en supportsag.</span><span class="sxs-lookup"><span data-stu-id="f136f-113">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="f136f-114">I mange tilfælde kan arbejder vi allerede på en løsning.</span><span class="sxs-lookup"><span data-stu-id="f136f-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="f136f-115">Giv os, mindst 24 timer at gennemføre en løsning.</span><span class="sxs-lookup"><span data-stu-id="f136f-115">Please give us at least 24 hours to complete a solution.</span></span>

<span data-ttu-id="f136f-116">**Vigtigt**: Hvis et websted, dokument (bibliotek) eller en liste blev slettet og stadig vises i søgeresultaterne, brugere skal modtage en fejl 404-filen blev ikke fundet under forsøg på at få adgang til.</span><span class="sxs-lookup"><span data-stu-id="f136f-116">**Important**: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an Error 404 File Not Found when trying to access.</span></span> <span data-ttu-id="f136f-117">Dette problem bør registreres som en supportsag til yderligere undersøgelse.</span><span class="sxs-lookup"><span data-stu-id="f136f-117">This issue should be logged as a support case for further investigation.</span></span> 



