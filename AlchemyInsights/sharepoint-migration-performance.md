---
title: SharePoint-overførselsydeevne
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "2700"
ms.openlocfilehash: 812444589d5a5bf766bbc6f466077d4ca829d79f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931998"
---
# <a name="sharepoint-migration-performance"></a><span data-ttu-id="b6c7a-102">SharePoint-overførselsydeevne</span><span class="sxs-lookup"><span data-stu-id="b6c7a-102">SharePoint migration performance</span></span>

<span data-ttu-id="b6c7a-103">**Vigtigt**: Mange SharePoint Online- og OneDrive-kunder kører forretningskritiske programmer op mod tjenesten, der kører i baggrunden.</span><span class="sxs-lookup"><span data-stu-id="b6c7a-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="b6c7a-104">Disse omfatter indholdsoverførsel, forebyggelse af datatab (DLP) og løsninger til sikkerhedskopiering.</span><span class="sxs-lookup"><span data-stu-id="b6c7a-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="b6c7a-105">I disse hidtil usete tider tager vi skridt til at sikre, at SharePoint Online- og OneDrive-tjenester forbliver meget tilgængelige og pålidelige for dine brugere, der er mere afhængige af din tjeneste end nogensinde før i fjernarbejdssituationer.</span><span class="sxs-lookup"><span data-stu-id="b6c7a-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="b6c7a-106">For at understøtte denne målsætning har vi implementeret strengere begrænsninger for baggrundsapps (overførsel, DLP og løsninger til sikkerhedskopiering) i dagtimerne på hverdage.</span><span class="sxs-lookup"><span data-stu-id="b6c7a-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="b6c7a-107">Du bør forvente, at disse apps vil opnå en meget begrænset dataoverførselshastighed i disse tidsrum.</span><span class="sxs-lookup"><span data-stu-id="b6c7a-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="b6c7a-108">Derimod vil tjenesten i løbet af aften- og weekendtimerne i dit område være klar til at behandle en betydeligt højere mængde forespørgsler fra baggrundsapps.</span><span class="sxs-lookup"><span data-stu-id="b6c7a-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="b6c7a-109">**Overførselsydeevne**</span><span class="sxs-lookup"><span data-stu-id="b6c7a-109">**Migration performance**</span></span>

<span data-ttu-id="b6c7a-110">Overførselsydeevnen kan blive påvirket af netværksinfrastruktur, filstørrelse, overførselstid og begrænsning.</span><span class="sxs-lookup"><span data-stu-id="b6c7a-110">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling.</span></span> <span data-ttu-id="b6c7a-111">At forstå disse faktorer vil hjælpe dig med at planlægge og maksimere din overførsels effektivitet.</span><span class="sxs-lookup"><span data-stu-id="b6c7a-111">Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

<span data-ttu-id="b6c7a-112">Besøg nedenstående links for at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="b6c7a-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="b6c7a-113">Overførselshastighed for SharePoint Online og ODB</span><span class="sxs-lookup"><span data-stu-id="b6c7a-113">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="b6c7a-114">Undgå at blive begrænset eller blokeret i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="b6c7a-114">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="b6c7a-115">Download og installer Migreringsværktøj til SharePoint</span><span class="sxs-lookup"><span data-stu-id="b6c7a-115">Download and install the SharePoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)
