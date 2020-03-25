---
title: Fejlfinding i forbindelse med problemer og fejl i SharePoint-overførselsværktøjet
ms.author: v-miegge
author: v-miegge
manager: v-cojank
ms.date: 10/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3178"
ms.assetid: ''
ms.openlocfilehash: f9f5694b1d88bccebdc5448d5629ea5120c52511
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931112"
---
# <a name="troubleshooting-sharepoint-migration-tool-issues-and-errors"></a><span data-ttu-id="bb05b-102">Fejlfinding i forbindelse med problemer og fejl i SharePoint-overførselsværktøjet</span><span class="sxs-lookup"><span data-stu-id="bb05b-102">Troubleshooting SharePoint Migration Tool issues and errors</span></span>

<span data-ttu-id="bb05b-103">**Vigtigt**: Mange SharePoint Online- og OneDrive-kunder kører forretningskritiske programmer mod den tjeneste, der kører i baggrunden.</span><span class="sxs-lookup"><span data-stu-id="bb05b-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="bb05b-104">Disse omfatter indholdsmigrering, Forebyggelse af datatab (DLP) og sikkerhedskopieringsløsninger.</span><span class="sxs-lookup"><span data-stu-id="bb05b-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="bb05b-105">I disse hidtil usete tider tager vi skridt til at sikre, at SharePoint Online- og OneDrive-tjenester forbliver meget tilgængelige og pålidelige for dine brugere, der er afhængige af tjenesten mere end nogensinde før i scenarier for fjernarbejde.</span><span class="sxs-lookup"><span data-stu-id="bb05b-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="bb05b-106">Til støtte for dette mål har vi implementeret strammere begrænsningsgrænser for baggrundsapps (migrering, DLP og backupløsninger) i dagtimerne på hverdage.</span><span class="sxs-lookup"><span data-stu-id="bb05b-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="bb05b-107">Du bør forvente, at disse apps vil opnå meget begrænset gennemløb i disse tider.</span><span class="sxs-lookup"><span data-stu-id="bb05b-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="bb05b-108">I løbet af aftenen og i weekenden for regionen vil tjenesten dog være klar til at behandle en betydeligt større mængde anmodninger fra baggrundsapps.</span><span class="sxs-lookup"><span data-stu-id="bb05b-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="bb05b-109">**Almindelige problemer og fejl**</span><span class="sxs-lookup"><span data-stu-id="bb05b-109">**Common issues and errors**</span></span>

<span data-ttu-id="bb05b-110">Der kan opstå almindelige problemer og fejl, når du bruger SPMT (SharePoint Migration Tool).</span><span class="sxs-lookup"><span data-stu-id="bb05b-110">You may encounter some common issues and errors when using the SharePoint Migration Tool (SPMT).</span></span> <span data-ttu-id="bb05b-111">Se nedenstående links for at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="bb05b-111">Please reference the links below for more information.</span></span>

* [<span data-ttu-id="bb05b-112">Fejlfinding i forbindelse med almindelige SPMT-problemer og -fejl</span><span class="sxs-lookup"><span data-stu-id="bb05b-112">Troubleshooting common SPMT issues and errors</span></span>](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
* [<span data-ttu-id="bb05b-113">Fejlfinding i forbindelse med installationsproblemer med SPMT</span><span class="sxs-lookup"><span data-stu-id="bb05b-113">Troubleshooting SPMT install issues</span></span>](https://docs.microsoft.com/sharepointmigration/spmt-install-issues)