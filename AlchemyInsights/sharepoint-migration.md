---
title: Overføre indstillinger til SharePoint Online
ms.author: pebaum
author: v-miegge
manager: v-cojank
ms.date: 11/04/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: c8c339c9-2e50-4daa-aa91-3eb5053e2bc6
ms.openlocfilehash: 830b39c51658cbc02f4be81acdfdf3b164a8df70
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932724"
---
# <a name="migrate-options-to-sharepoint-online"></a><span data-ttu-id="4aa70-102">Overføre indstillinger til SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="4aa70-102">Migrate options to SharePoint Online</span></span>

<span data-ttu-id="4aa70-103">**Vigtigt**: Mange SharePoint Online- og OneDrive-kunder kører forretningskritiske programmer mod den tjeneste, der kører i baggrunden.</span><span class="sxs-lookup"><span data-stu-id="4aa70-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="4aa70-104">Disse omfatter indholdsmigrering, Forebyggelse af datatab (DLP) og sikkerhedskopieringsløsninger.</span><span class="sxs-lookup"><span data-stu-id="4aa70-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="4aa70-105">I disse hidtil usete tider tager vi skridt til at sikre, at SharePoint Online- og OneDrive-tjenester forbliver meget tilgængelige og pålidelige for dine brugere, der er afhængige af tjenesten mere end nogensinde før i scenarier for fjernarbejde.</span><span class="sxs-lookup"><span data-stu-id="4aa70-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="4aa70-106">Til støtte for dette mål har vi implementeret strammere begrænsningsgrænser for baggrundsapps (migrering, DLP og backupløsninger) i dagtimerne på hverdage.</span><span class="sxs-lookup"><span data-stu-id="4aa70-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="4aa70-107">Du bør forvente, at disse apps vil opnå meget begrænset gennemløb i disse tider.</span><span class="sxs-lookup"><span data-stu-id="4aa70-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="4aa70-108">I løbet af aftenen og i weekenden for regionen vil tjenesten dog være klar til at behandle en betydeligt større mængde anmodninger fra baggrundsapps.</span><span class="sxs-lookup"><span data-stu-id="4aa70-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="4aa70-109">**Indstillinger for overflytning**</span><span class="sxs-lookup"><span data-stu-id="4aa70-109">**Migration options**</span></span>

<span data-ttu-id="4aa70-110">Der er forskellige muligheder for at overføre indhold til SharePoint Online, afhængigt af størrelsen og mængden af filer, du skal flytte, se en liste over [muligheder, der er placeret her](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="4aa70-110">There are different options available to migrate content to SharePoint Online, depending on the size and quantity of files you need to move, please see a list of options [located here](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span></span>

<span data-ttu-id="4aa70-111">Du kan finde flere oplysninger om indholdsmigrering på nedenstående links.</span><span class="sxs-lookup"><span data-stu-id="4aa70-111">For more information on content migration, please visit the links below.</span></span>

- [<span data-ttu-id="4aa70-112">Værktøjet Til overførsel af Sharepoint</span><span class="sxs-lookup"><span data-stu-id="4aa70-112">Sharepoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)

- [<span data-ttu-id="4aa70-113">Introduktion til Overførselsstyring</span><span class="sxs-lookup"><span data-stu-id="4aa70-113">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="4aa70-114">Hastighed for Sharepoint Online- og ODB-overførsel</span><span class="sxs-lookup"><span data-stu-id="4aa70-114">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="4aa70-115">Undgå at få gaseller blokeret i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="4aa70-115">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="4aa70-116">SMAT (SharePoint Migration Assessment Tool)</span><span class="sxs-lookup"><span data-stu-id="4aa70-116">SharePoint Migration Assessment Tool (SMAT)</span></span>](https://www.microsoft.com/download/details.aspx?id=53598&amp;751be11f-ede8-5a0c-058c-2ee190a24fa6=True)

<span data-ttu-id="4aa70-117">**Bemærk:** I øjeblikket understøtter SharePoint-overførselsværktøjet kun overførsler fra SharePoint 2010 og 2013.</span><span class="sxs-lookup"><span data-stu-id="4aa70-117">**Note**: Currently the SharePoint Migration tool only support migrations from SharePoint 2010  and 2013.</span></span> <span data-ttu-id="4aa70-118">Version 2016 eller 2019 understøttes ikke på nuværende tidspunkt.</span><span class="sxs-lookup"><span data-stu-id="4aa70-118">Version 2016 or 2019 are not supported at this time.</span></span>
