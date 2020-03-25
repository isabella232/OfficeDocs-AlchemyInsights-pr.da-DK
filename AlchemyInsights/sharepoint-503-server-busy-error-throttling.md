---
title: Begrænsning af SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931220"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="29409-102">Begrænsning af SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="29409-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="29409-103">**Vigtigt**: Mange SharePoint Online- og OneDrive-kunder kører forretningskritiske programmer mod den tjeneste, der kører i baggrunden.</span><span class="sxs-lookup"><span data-stu-id="29409-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="29409-104">Disse omfatter indholdsmigrering, Forebyggelse af datatab (DLP) og sikkerhedskopieringsløsninger.</span><span class="sxs-lookup"><span data-stu-id="29409-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="29409-105">I disse hidtil usete tider tager vi skridt til at sikre, at SharePoint Online- og OneDrive-tjenester forbliver meget tilgængelige og pålidelige for dine brugere, der er afhængige af tjenesten mere end nogensinde før i scenarier for fjernarbejde.</span><span class="sxs-lookup"><span data-stu-id="29409-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="29409-106">Til støtte for dette mål har vi implementeret strammere begrænsningsgrænser for baggrundsapps (migrering, DLP og backupløsninger) i dagtimerne på hverdage.</span><span class="sxs-lookup"><span data-stu-id="29409-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="29409-107">Du bør forvente, at disse apps vil opnå meget begrænset gennemløb i disse tider.</span><span class="sxs-lookup"><span data-stu-id="29409-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="29409-108">I løbet af aftenen og i weekenden for regionen vil tjenesten dog være klar til at behandle en betydeligt større mængde anmodninger fra baggrundsapps.</span><span class="sxs-lookup"><span data-stu-id="29409-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="29409-109">**503-serveren er optaget**</span><span class="sxs-lookup"><span data-stu-id="29409-109">**503 server is busy error**</span></span>

<span data-ttu-id="29409-110">Brugerne får muligvis vist en 503-server, der er optaget, når de forsøger at navigere til SharePoint- eller OneDrive-websteder.</span><span class="sxs-lookup"><span data-stu-id="29409-110">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="29409-111">Denne fejl kan skyldes begrænsning i SharePoint-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="29409-111">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="29409-112">SharePoint Online bruger begrænsning til at opretholde optimal ydeevne og pålidelighed i SharePoint Online-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="29409-112">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="29409-113">Begrænsning begrænser antallet af brugerhandlinger eller samtidige opkald (efter script eller kode) for at forhindre overforbrug af ressourcer.</span><span class="sxs-lookup"><span data-stu-id="29409-113">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="29409-114">Du kan finde flere oplysninger om begrænsning under [Undgå at blive kvalt eller blokeret i SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="29409-114">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="29409-115">Hvis du mener, at denne fejl ikke er relateret til begrænsning, kan du kontrollere, om der er aktiv vedligeholdelse på din lejer, ved at navigere til [Meddelelsescenter](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="29409-115">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="29409-116">Endelig skal du sørge for at besøge [siden Tjenestetilstand](https://portal.office.com/adminportal/home#/servicehealth) for at kontrollere, om der er råd/hændelser, der måtte forekomme.</span><span class="sxs-lookup"><span data-stu-id="29409-116">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

