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
ms.openlocfilehash: c7881c0c7331e0aa74fcc439f52157bb75a56160
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559834"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="35ec1-102">Begrænsning af SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="35ec1-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="35ec1-103">Brugere kan få vist en 503 serveren er optaget fejl, når du forsøger at navigere til websteder, SharePoint- eller OneDrive.</span><span class="sxs-lookup"><span data-stu-id="35ec1-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="35ec1-104">Denne fejl kan være forårsaget af begrænsning i SharePoint-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="35ec1-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="35ec1-105">SharePoint Online anvender throttling for at vedligeholde optimal ydeevne og pålidelighed af SharePoint Online-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="35ec1-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="35ec1-106">Begrænsning af grænser opkald antallet af brugerhandlinger eller samtidige (ved script eller kode) for at undgå merforbrug af ressourcer.</span><span class="sxs-lookup"><span data-stu-id="35ec1-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="35ec1-107">Hvis du få begrænset, 99% af den tid, det er på grund af brugerdefineret kode.</span><span class="sxs-lookup"><span data-stu-id="35ec1-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="35ec1-108">Yderligere oplysninger om begrænsning af finder du [undgå at få begrænset eller blokeret i SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="35ec1-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="35ec1-109">Hvis du mener, at denne fejl ikke vedrører begrænsning, kan du kontrollere, om der findes aktive vedligeholdelse, der forekommer på din lejer ved at gå til [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="35ec1-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="35ec1-110">Endelig skal du kontrollere du besøger siden [Service sundhed](https://portal.office.com/adminportal/home#/servicehealth) til at kontrollere for eventuelle sikkerhedsmeddelelser/hændelser, der kan forekomme.</span><span class="sxs-lookup"><span data-stu-id="35ec1-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

