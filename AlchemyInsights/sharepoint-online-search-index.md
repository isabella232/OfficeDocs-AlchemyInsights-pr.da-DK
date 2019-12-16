---
title: Søg i SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c4ff98f0cf928834c803542340b32da15a40d583
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40044037"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="73daf-102">Indholds gennemsøgning og indeksering i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="73daf-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="73daf-103">Indholdet skal crawlede og føjes til søgeindekset, for at brugerne kan finde det, de søger efter, i SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="73daf-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="73daf-104">Indhold gennemsøges automatisk ud fra en foruddefineret tidsplan (gennemsøgnings planen kan ikke ændres).</span><span class="sxs-lookup"><span data-stu-id="73daf-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="73daf-105">Crawleren henter indhold, der er ændret siden sidste gennemsøgning, og opdaterer indekset.</span><span class="sxs-lookup"><span data-stu-id="73daf-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="73daf-106">Bemærk følgende for at sikre, at indholdet gennemsøges, og indekset opdateres:</span><span class="sxs-lookup"><span data-stu-id="73daf-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="73daf-107">Sørg for, at indhold kan findes ved [at gøre webstedsindhold søgbart](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="73daf-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="73daf-108">Når du har ændret en administreret egenskab, eller når du har ændret tilknytningen af gennemsøgte og administrerede egenskaber, skal webstedet crawles igen, før ændringerne afspejles i søgeindekset.</span><span class="sxs-lookup"><span data-stu-id="73daf-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="73daf-109">Da dine ændringer foretages i søgeskemaet og ikke på det faktiske websted, indekseres webcrawleren ikke automatisk webstedet igen.</span><span class="sxs-lookup"><span data-stu-id="73daf-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="73daf-110">Du kan finde flere oplysninger under [Manuel anmodning om gennemsøgning og genindekse ring af et websted, et bibliotek eller en liste](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="73daf-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="73daf-111">Vent mindst 24 timer efter, at du manuelt har anmodet om en gennemsøgning og et fuldstændigt genindeks for at se, om du stadig oplever et problem.</span><span class="sxs-lookup"><span data-stu-id="73daf-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="73daf-112">Hvis der er gået mere end 24 timer, siden du indledte gennemsøgningen og fuld re-index, skal du logge en support sag.</span><span class="sxs-lookup"><span data-stu-id="73daf-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="73daf-113">I mange tilfælde arbejder vi allerede på en løsning.</span><span class="sxs-lookup"><span data-stu-id="73daf-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="73daf-114">Giv os mindst 24 timer til at gennemføre en løsning.</span><span class="sxs-lookup"><span data-stu-id="73daf-114">Please give us at least 24 hours to complete a solution.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="73daf-115">Hvis et websted, dokument (bibliotek) eller en liste er blevet slettet og stadig vises i søgeresultaterne, skal brugerne modtage en **fejl 404-fil, der ikke blev fundet** , da de forsøgte at få adgang til den.</span><span class="sxs-lookup"><span data-stu-id="73daf-115">If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="73daf-116">Dette spørgsmål skal registreres som en støtte sag for yderligere undersøgelse.</span><span class="sxs-lookup"><span data-stu-id="73daf-116">This issue should be logged as a support case for further investigation.</span></span> 



