---
title: Problemer med ydeevnen-SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068390"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="7a018-102">SharePoint eller OneDrive langsom, utilgængelig eller utilgængelig for flere brugere</span><span class="sxs-lookup"><span data-stu-id="7a018-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="7a018-103">SharePoint eller OneDrive kan være langsomme, utilgængelige eller utilgængelige eller kan vise tjenesten utilgængelig eller 503 fejl af flere årsager:</span><span class="sxs-lookup"><span data-stu-id="7a018-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="7a018-104">Hvis dit SharePoint-eller OneDrive-websted er langsomt eller forsinket for flere brugere, kan der være et midlertidigt serviceproblem, hvor brugere oplever periodiske forsinkelser eller navigationsfejl, når de får adgang til SharePoint-websteder eller OneDrive-indhold.</span><span class="sxs-lookup"><span data-stu-id="7a018-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="7a018-105">Kontroller [dashboardet for tjenestetilstand](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) for at se, om din organisation påvirkes.</span><span class="sxs-lookup"><span data-stu-id="7a018-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="7a018-106">Brugere kan modtage en *503 server er optaget* fejl, når de forsøger at navigere til SharePoint eller OneDrive sites.</span><span class="sxs-lookup"><span data-stu-id="7a018-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="7a018-107">Denne fejl kan forårsages af begrænsning i SharePoint-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="7a018-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="7a018-108">SharePoint Online brugerbegrænsning til at opretholde den optimale ydeevne og pålidelighed af SharePoint Online-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="7a018-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="7a018-109">Throttling begrænser antallet af brugerhandlinger eller samtidige kald (efter script eller kode) for at forhindre overforbrug af ressourcer.</span><span class="sxs-lookup"><span data-stu-id="7a018-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="7a018-110">Du finder flere oplysninger om begrænsning under Se ved at [undgå at blive begrænset eller blokeret i SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="7a018-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="7a018-111">Hvis du oplever langsom ydeevne med et **klassisk** eller **moderne** SharePoint-websted eller-side, skal du bruge [værktøjet til side diagnosticering](https://aka.ms/perftool) til at analysere siderne.</span><span class="sxs-lookup"><span data-stu-id="7a018-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="7a018-112">Hvis du stadig oplever generel langsom ydeevne, skal du gennemse ressourcerne nederst i denne artikel: [Introduktion til justering af ydeevnen for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="7a018-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  