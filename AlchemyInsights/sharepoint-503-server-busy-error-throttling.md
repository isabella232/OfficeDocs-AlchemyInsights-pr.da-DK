---
title: Begrænsning af SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 50b2c29db1fd294abe6c9e60f067156109de392b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742203"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="dc267-102">Begrænsning af SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="dc267-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="dc267-103">**Vigtigt**: I disse hidtil usete tider bestræber vi os på at sikre, at SharePoint Online- og OneDrive-tjenesterne fastholder sin høje tilgængelighed. Hvis du ønsker flere oplysninger, skal du besøge [Midlertidige funktionsjusteringer i SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="dc267-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="dc267-104">**503-serveren er optaget**</span><span class="sxs-lookup"><span data-stu-id="dc267-104">**503 server is busy error**</span></span>

<span data-ttu-id="dc267-105">Brugerne får muligvis vist en 503-server, der er optaget, når de forsøger at navigere til SharePoint- eller OneDrive-websteder.</span><span class="sxs-lookup"><span data-stu-id="dc267-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="dc267-106">Denne fejl kan skyldes begrænsning i SharePoint-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="dc267-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="dc267-107">SharePoint Online anvender begrænsning til at opretholde optimal ydeevne og pålidelighed for SharePoint Online-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="dc267-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="dc267-108">Begrænsning begrænser antallet af brugerhandlinger eller samtidige kald (via script eller kode) for at forhindre overbelastning af ressourcer.</span><span class="sxs-lookup"><span data-stu-id="dc267-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="dc267-109">Du kan finde flere oplysninger om begrænsning under [Undgå at blive kvalt eller blokeret i SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="dc267-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="dc267-110">Hvis du mener, at denne fejl ikke er relateret til begrænsning, kan du kontrollere, om der er aktiv vedligeholdelse på din lejer, ved at navigere til [Meddelelsescenter](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="dc267-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="dc267-111">Endelig skal du sørge for at besøge [siden Tjenestetilstand](https://portal.office.com/adminportal/home#/servicehealth) for at kontrollere, om der er råd/hændelser, der måtte forekomme.</span><span class="sxs-lookup"><span data-stu-id="dc267-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

