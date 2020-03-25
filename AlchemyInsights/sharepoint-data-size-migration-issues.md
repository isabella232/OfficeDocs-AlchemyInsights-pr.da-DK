---
title: Problemer under overførsel af data til SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "1885"
ms.openlocfilehash: b53a98480bab48497274c7358f7e606caa477f5a
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931688"
---
# <a name="issues-while-migrating-data-to-sharepoint-online"></a><span data-ttu-id="79ebd-102">Problemer under overførsel af data til SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="79ebd-102">Issues while migrating data to SharePoint Online</span></span>

<span data-ttu-id="79ebd-103">**Vigtigt**: Mange SharePoint Online- og OneDrive-kunder kører forretningskritiske programmer mod den tjeneste, der kører i baggrunden.</span><span class="sxs-lookup"><span data-stu-id="79ebd-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="79ebd-104">Disse omfatter indholdsmigrering, Forebyggelse af datatab (DLP) og sikkerhedskopieringsløsninger.</span><span class="sxs-lookup"><span data-stu-id="79ebd-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="79ebd-105">I disse hidtil usete tider tager vi skridt til at sikre, at SharePoint Online- og OneDrive-tjenester forbliver meget tilgængelige og pålidelige for dine brugere, der er afhængige af tjenesten mere end nogensinde før i scenarier for fjernarbejde.</span><span class="sxs-lookup"><span data-stu-id="79ebd-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="79ebd-106">Til støtte for dette mål har vi implementeret strammere begrænsningsgrænser for baggrundsapps (migrering, DLP og backupløsninger) i dagtimerne på hverdage.</span><span class="sxs-lookup"><span data-stu-id="79ebd-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="79ebd-107">Du bør forvente, at disse apps vil opnå meget begrænset gennemløb i disse tider.</span><span class="sxs-lookup"><span data-stu-id="79ebd-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="79ebd-108">I løbet af aftenen og i weekenden for regionen vil tjenesten dog være klar til at behandle en betydeligt større mængde anmodninger fra baggrundsapps.</span><span class="sxs-lookup"><span data-stu-id="79ebd-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="79ebd-109">**Overflytning af over 100 TB data**</span><span class="sxs-lookup"><span data-stu-id="79ebd-109">**Migrating over 100TB of data**</span></span>

<span data-ttu-id="79ebd-110">Det ser ud til, at du overfører over 100 TB data til SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="79ebd-110">It appears you are migrating over 100TB of data to SharePoint Online.</span></span> <span data-ttu-id="79ebd-111">Følg nedenstående trin, så vi kan hjælpe dig så hurtigt som muligt.</span><span class="sxs-lookup"><span data-stu-id="79ebd-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="79ebd-112">Vælg **Ny serviceanmodning**, og vælg derefter **Ny serviceanmodning**.</span><span class="sxs-lookup"><span data-stu-id="79ebd-112">Select **New Service Request**, and then **New Service Request**.</span></span> 
2. <span data-ttu-id="79ebd-113">Lad titlen og beskrivelsen være **SharePoint-overførsel over 100 TB**.</span><span class="sxs-lookup"><span data-stu-id="79ebd-113">Leave the title and description as **SharePoint migration over 100TB**.</span></span>
3. <span data-ttu-id="79ebd-114">Når billetten er indsendt, skal du opdatere den med følgende oplysninger:</span><span class="sxs-lookup"><span data-stu-id="79ebd-114">Once the ticket has been submitted, please update it with the following information:</span></span> 

    - <span data-ttu-id="79ebd-115">Anslået størrelse på din overførsel.</span><span class="sxs-lookup"><span data-stu-id="79ebd-115">Estimated size of your migration.</span></span>
    - <span data-ttu-id="79ebd-116">Et estimat over, hvornår du vil starte og fuldføre overførslen.</span><span class="sxs-lookup"><span data-stu-id="79ebd-116">An estimate of when you would like to start and complete your migration.</span></span>
    - <span data-ttu-id="79ebd-117">Beskriv, hvor du overfører dit indhold fra, f.eks.</span><span class="sxs-lookup"><span data-stu-id="79ebd-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>


  

