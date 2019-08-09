---
title: Administrere search-skema i SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f49195bec64f115063ccfb5256e27fbecd4a54f6
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270092"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="73d3a-102">Administrere search-skema i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="73d3a-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="73d3a-103">Search-skema styrer, hvad brugerne kan søge efter, hvordan brugerne kan søge i den, og hvordan du kan præsentere resultaterne på din søgning websteder.</span><span class="sxs-lookup"><span data-stu-id="73d3a-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="73d3a-104">Se [Manage Search-skema i SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) for at lære, hvordan du:</span><span class="sxs-lookup"><span data-stu-id="73d3a-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="73d3a-105">Ændre search-skema.</span><span class="sxs-lookup"><span data-stu-id="73d3a-105">Change the search schema.</span></span>
- <span data-ttu-id="73d3a-106">Oprette administrerede egenskaber.</span><span class="sxs-lookup"><span data-stu-id="73d3a-106">Create managed properties.</span></span>
- <span data-ttu-id="73d3a-107">Datatilknytning gennemsøgte knytte gennemsøgte egenskaber til administrerede egenskaber.</span><span class="sxs-lookup"><span data-stu-id="73d3a-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="73d3a-108">Bemærk følgende med hensyn til administration af Search-skema:</span><span class="sxs-lookup"><span data-stu-id="73d3a-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="73d3a-109">Hvis du modtager en advarsel om **programmet afbrydes** , når du foretager en skemaændring af, det er kun midlertidige da service vedligeholdelse forekommer.</span><span class="sxs-lookup"><span data-stu-id="73d3a-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="73d3a-110">Hvis der er gået mere end 24 timer, og du stadig opleve advarslen, skal du logge en supportsag.</span><span class="sxs-lookup"><span data-stu-id="73d3a-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="73d3a-111">Når du ændrer administrerede egenskaber eller tilføje nye, træder ændringerne i kraft, når indholdet er blevet gennemsøgt igen.</span><span class="sxs-lookup"><span data-stu-id="73d3a-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="73d3a-112">I SharePoint Online sker gennemsøgning automatisk baseret på den definerede gennemsøgning tidsplan.</span><span class="sxs-lookup"><span data-stu-id="73d3a-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="73d3a-113">Hvis du vil sikre dig, at dine ændringer er gennemsøgt, kan du specifikt [anmodning at indeksere liste eller bibliotek](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="73d3a-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="73d3a-114">Se [Introduktion til Search-skema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/) for en komplet oversigt over Search-skema</span><span class="sxs-lookup"><span data-stu-id="73d3a-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


