---
title: Begrænsning af SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 9af4f09d50992c04a1f3d5a164093049a3ec3517
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931436"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="c4a75-102">Begrænsning af SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="c4a75-102">SharePoint Online throttling</span></span>

<span data-ttu-id="c4a75-103">**Vigtigt**: Mange SharePoint Online- og OneDrive-kunder kører forretningskritiske programmer mod den tjeneste, der kører i baggrunden.</span><span class="sxs-lookup"><span data-stu-id="c4a75-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="c4a75-104">Disse omfatter indholdsmigrering, Forebyggelse af datatab (DLP) og sikkerhedskopieringsløsninger.</span><span class="sxs-lookup"><span data-stu-id="c4a75-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="c4a75-105">I disse hidtil usete tider tager vi skridt til at sikre, at SharePoint Online- og OneDrive-tjenester forbliver meget tilgængelige og pålidelige for dine brugere, der er afhængige af tjenesten mere end nogensinde før i scenarier for fjernarbejde.</span><span class="sxs-lookup"><span data-stu-id="c4a75-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="c4a75-106">Til støtte for dette mål har vi implementeret strammere begrænsningsgrænser for baggrundsapps (migrering, DLP og backupløsninger) i dagtimerne på hverdage.</span><span class="sxs-lookup"><span data-stu-id="c4a75-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="c4a75-107">Du bør forvente, at disse apps vil opnå meget begrænset gennemløb i disse tider.</span><span class="sxs-lookup"><span data-stu-id="c4a75-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="c4a75-108">I løbet af aftenen og i weekenden for regionen vil tjenesten dog være klar til at behandle en betydeligt større mængde anmodninger fra baggrundsapps.</span><span class="sxs-lookup"><span data-stu-id="c4a75-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="c4a75-109">**Begrænsning af SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="c4a75-109">**SharePoint Online throttling**</span></span>

<span data-ttu-id="c4a75-110">SharePoint Online bruger begrænsning til at opretholde optimal ydeevne og pålidelighed i SharePoint Online-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="c4a75-110">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="c4a75-111">Begrænsning begrænser antallet af brugerhandlinger eller samtidige opkald (efter script eller kode) for at forhindre overforbrug af ressourcer.</span><span class="sxs-lookup"><span data-stu-id="c4a75-111">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="c4a75-112">For mere information, kan du besøge nedenstående links.</span><span class="sxs-lookup"><span data-stu-id="c4a75-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="c4a75-113">Undgå at få gaseller blokeret i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="c4a75-113">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="c4a75-114">Begrænsning af dataoverførsel og spobegrænsning</span><span class="sxs-lookup"><span data-stu-id="c4a75-114">Data Migration and SPO Throttling </span></span>](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)

- [<span data-ttu-id="c4a75-115">Hastighed for overførsel af SharePoint Online og OneDrive</span><span class="sxs-lookup"><span data-stu-id="c4a75-115">SharePoint Online and OneDrive Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

 - [<span data-ttu-id="c4a75-116">Håndtere Begrænsning af SharePoint Online ved hjælp af eksponentiel back off</span><span class="sxs-lookup"><span data-stu-id="c4a75-116">Handle SharePoint Online throttling by using exponential back off</span></span>](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)

- [<span data-ttu-id="c4a75-117">Kapacitetsplanlægning og belastningstest af SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="c4a75-117">Capacity planning and load testing SharePoint Online</span></span>](https://docs.microsoft.com/office365/enterprise/capacity-planning-and-load-testing-sharepoint-online)

