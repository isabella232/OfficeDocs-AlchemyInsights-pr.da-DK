---
title: SharePoint-overførsel med SPMT
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "2594"
ms.openlocfilehash: e7719d1fc6dda0d5bd340775219401dade2933fe
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931544"
---
# <a name="sharepoint-migration-with-spmt"></a><span data-ttu-id="dfff5-102">SharePoint-overførsel med SPMT</span><span class="sxs-lookup"><span data-stu-id="dfff5-102">SharePoint Migration with SPMT</span></span>

<span data-ttu-id="dfff5-103">**Vigtigt**: Mange SharePoint Online- og OneDrive-kunder kører forretningskritiske programmer mod den tjeneste, der kører i baggrunden.</span><span class="sxs-lookup"><span data-stu-id="dfff5-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="dfff5-104">Disse omfatter indholdsmigrering, Forebyggelse af datatab (DLP) og sikkerhedskopieringsløsninger.</span><span class="sxs-lookup"><span data-stu-id="dfff5-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="dfff5-105">I disse hidtil usete tider tager vi skridt til at sikre, at SharePoint Online- og OneDrive-tjenester forbliver meget tilgængelige og pålidelige for dine brugere, der er afhængige af tjenesten mere end nogensinde før i scenarier for fjernarbejde.</span><span class="sxs-lookup"><span data-stu-id="dfff5-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="dfff5-106">Til støtte for dette mål har vi implementeret strammere begrænsningsgrænser for baggrundsapps (migrering, DLP og backupløsninger) i dagtimerne på hverdage.</span><span class="sxs-lookup"><span data-stu-id="dfff5-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="dfff5-107">Du bør forvente, at disse apps vil opnå meget begrænset gennemløb i disse tider.</span><span class="sxs-lookup"><span data-stu-id="dfff5-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="dfff5-108">I løbet af aftenen og i weekenden for regionen vil tjenesten dog være klar til at behandle en betydeligt større mængde anmodninger fra baggrundsapps.</span><span class="sxs-lookup"><span data-stu-id="dfff5-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="dfff5-109">**VÃ¦rktÃ ̧jet til Overflytning af SharePoint**</span><span class="sxs-lookup"><span data-stu-id="dfff5-109">**SharePoint Migration Tool**</span></span>

<span data-ttu-id="dfff5-110">SharePoint Migration Tool er designet til at blive brugt til overførsler, der spænder fra det mindste sæt filer til en storstilet virksomhedsmigrering, og giver dig mulighed for at overføre dine oplysninger til skyen og drage fordel af det nyeste samarbejde, den nyeste intelligens og sikkerhedsløsninger med Office 365.</span><span class="sxs-lookup"><span data-stu-id="dfff5-110">Designed to be used for migrations ranging from the smallest set of files to a large scale enterprise migration, the SharePoint Migration Tool will allow you to transfer your information to the cloud and take advantage of the newest collaboration, intelligence, and security solutions with Office 365.</span></span>

- [<span data-ttu-id="dfff5-111">Hente og installere SharePoint-overførselsværktøjet</span><span class="sxs-lookup"><span data-stu-id="dfff5-111">Download and install the SharePoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)
- [<span data-ttu-id="dfff5-112">Fejlfinding i forbindelse med almindelige SPMT-problemer og -fejl</span><span class="sxs-lookup"><span data-stu-id="dfff5-112">Troubleshooting common SPMT issues and errors</span></span>](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
- [<span data-ttu-id="dfff5-113">Fejlfinding i forbindelse med SPMT-installationsproblemer</span><span class="sxs-lookup"><span data-stu-id="dfff5-113">Troubleshooting SPMT installation issues</span></span>](https://docs.microsoft.com/sharepointmigration/spmt-install-issues#troubleshooting-spmt-installation-issues)
