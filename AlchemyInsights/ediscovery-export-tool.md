---
title: eDiscovery-eksportværktøj
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814582"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="186e5-102">Kan du ikke installere eller køre eDiscovery-eksportværktøjet?</span><span class="sxs-lookup"><span data-stu-id="186e5-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="186e5-103">Hvis du ikke kan installere eller køre eDiscovery-eksportværktøjet for at hente søgeresultater, skal du kontrollere følgende:</span><span class="sxs-lookup"><span data-stu-id="186e5-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="186e5-104">Den computer, du bruger, opfylder følgende forudsætninger:</span><span class="sxs-lookup"><span data-stu-id="186e5-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="186e5-105">32- eller 64-bit versioner af Windows 7 og nyere versioner</span><span class="sxs-lookup"><span data-stu-id="186e5-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="186e5-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="186e5-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="186e5-107">En understøttet browser:</span><span class="sxs-lookup"><span data-stu-id="186e5-107">A supported browser:</span></span>

  - <span data-ttu-id="186e5-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="186e5-108">Microsoft Edge</span></span>

    <span data-ttu-id="186e5-109">Eller</span><span class="sxs-lookup"><span data-stu-id="186e5-109">Or</span></span>

  - <span data-ttu-id="186e5-110">Internet Explorer 10 og nyere versioner</span><span class="sxs-lookup"><span data-stu-id="186e5-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="186e5-111">Andre browsere, f.eks Google Chrome og Mozilla Firefox, understøttes ikke.</span><span class="sxs-lookup"><span data-stu-id="186e5-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="186e5-112">Din organisation kan oprette forbindelse til slutpunktet i Azure, som er **\* .blob.core.windows.net** (jokertegnet repræsenterer et entydig identifier for dit eksportjob).</span><span class="sxs-lookup"><span data-stu-id="186e5-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="186e5-113">Du er tildelt Eksport-rollen i Microsoft 365 Security &amp; Compliance Center.</span><span class="sxs-lookup"><span data-stu-id="186e5-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="186e5-114">Som standard er denne rolle kun tildelt rollegruppen eDiscovery Manager.</span><span class="sxs-lookup"><span data-stu-id="186e5-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="186e5-115">Se [Tildel eDiscovery-tilladelser](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span><span class="sxs-lookup"><span data-stu-id="186e5-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="186e5-116">Få mere at vide under [Eksportér resultater fra indholdssøgning.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)</span><span class="sxs-lookup"><span data-stu-id="186e5-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="186e5-117">Hvis du eksporterer mere end 100.000 postkasser, skal du bruge følgende Powershell til at hente eksportresultaterne: Eksport af resultater fra mere end [100.000 postkasser.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)</span><span class="sxs-lookup"><span data-stu-id="186e5-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>