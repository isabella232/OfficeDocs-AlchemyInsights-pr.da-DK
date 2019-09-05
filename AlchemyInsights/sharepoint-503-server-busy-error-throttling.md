---
title: SharePoint Online-throttling
ms.author: pebaum
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: d9e1400697b1e6435fea78703d2ecadc6733a57f
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751882"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="13bef-102">SharePoint Online-throttling</span><span class="sxs-lookup"><span data-stu-id="13bef-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="13bef-103">Brugere kan modtage en 503 server er optaget fejl, når de forsøger at navigere til SharePoint eller OneDrive sites.</span><span class="sxs-lookup"><span data-stu-id="13bef-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="13bef-104">Denne fejl kan forårsages af begrænsning i SharePoint-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="13bef-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="13bef-105">SharePoint Online brugerbegrænsning til at opretholde den optimale ydeevne og pålidelighed af SharePoint Online-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="13bef-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="13bef-106">Throttling begrænser antallet af brugerhandlinger eller samtidige kald (efter script eller kode) for at forhindre overforbrug af ressourcer.</span><span class="sxs-lookup"><span data-stu-id="13bef-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="13bef-107">Hvis du får throttled, 99% af tiden er det på grund af brugerdefineret kode.</span><span class="sxs-lookup"><span data-stu-id="13bef-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="13bef-108">Du finder flere oplysninger om begrænsning under Se ved at [undgå at blive begrænset eller blokeret i SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="13bef-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="13bef-109">Hvis du mener, at denne fejl ikke er relateret til throttling, kan du kontrollere, om der er aktiv vedligeholdelse på din lejer, ved at navigere til [meddelelsescenteret](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="13bef-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="13bef-110">Endelig skal du sikre dig, at du besøger siden [tjenestetilstand](https://portal.office.com/adminportal/home#/servicehealth) for at kontrollere, om der er meddelelser/hændelser, som kan forekomme.</span><span class="sxs-lookup"><span data-stu-id="13bef-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

