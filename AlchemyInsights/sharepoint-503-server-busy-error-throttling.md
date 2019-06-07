---
title: Begrænsning af SharePoint Online
ms.author: kirks
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: b157ce22962ac1616d6e9b3a5475edaec7fed9f7
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/07/2019
ms.locfileid: "34761253"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="0a138-102">Begrænsning af SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="0a138-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="0a138-103">Brugere kan få vist en 503 serveren er optaget fejl, når du forsøger at navigere til websteder, SharePoint- eller OneDrive.</span><span class="sxs-lookup"><span data-stu-id="0a138-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="0a138-104">Denne fejl kan være forårsaget af begrænsning i SharePoint-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="0a138-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="0a138-105">SharePoint Online anvender throttling for at vedligeholde optimal ydeevne og pålidelighed af SharePoint Online-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="0a138-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="0a138-106">Begrænsning af grænser opkald antallet af brugerhandlinger eller samtidige (ved script eller kode) for at undgå merforbrug af ressourcer.</span><span class="sxs-lookup"><span data-stu-id="0a138-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="0a138-107">Hvis du få begrænset, 99% af den tid, det er på grund af brugerdefineret kode.</span><span class="sxs-lookup"><span data-stu-id="0a138-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="0a138-108">Yderligere oplysninger om begrænsning af finder du [undgå at få begrænset eller blokeret i SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="0a138-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="0a138-109">Hvis du mener, at denne fejl ikke vedrører begrænsning, kan du kontrollere, om der findes aktive vedligeholdelse, der forekommer på din lejer ved at gå til [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="0a138-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="0a138-110">Endelig skal du kontrollere du besøger siden [Service sundhed](https://portal.office.com/adminportal/home#/servicehealth) til at kontrollere for eventuelle sikkerhedsmeddelelser/hændelser, der kan forekomme.</span><span class="sxs-lookup"><span data-stu-id="0a138-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

