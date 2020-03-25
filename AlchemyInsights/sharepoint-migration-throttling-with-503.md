---
title: Begrænsning af SharePoint-overførsel med 503-fejl
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931652"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a><span data-ttu-id="79c76-102">Begrænsning af SharePoint-overførsel med 503-fejl</span><span class="sxs-lookup"><span data-stu-id="79c76-102">SharePoint migration throttling with 503 errors</span></span>

<span data-ttu-id="79c76-103">**Vigtigt**: Mange SharePoint Online- og OneDrive-kunder kører forretningskritiske programmer mod den tjeneste, der kører i baggrunden.</span><span class="sxs-lookup"><span data-stu-id="79c76-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="79c76-104">Disse omfatter indholdsmigrering, Forebyggelse af datatab (DLP) og sikkerhedskopieringsløsninger.</span><span class="sxs-lookup"><span data-stu-id="79c76-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="79c76-105">I disse hidtil usete tider tager vi skridt til at sikre, at SharePoint Online- og OneDrive-tjenester forbliver meget tilgængelige og pålidelige for dine brugere, der er afhængige af tjenesten mere end nogensinde før i scenarier for fjernarbejde.</span><span class="sxs-lookup"><span data-stu-id="79c76-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="79c76-106">Til støtte for dette mål har vi implementeret strammere begrænsningsgrænser for baggrundsapps (migrering, DLP og backupløsninger) i dagtimerne på hverdage.</span><span class="sxs-lookup"><span data-stu-id="79c76-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="79c76-107">Du bør forvente, at disse apps vil opnå meget begrænset gennemløb i disse tider.</span><span class="sxs-lookup"><span data-stu-id="79c76-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="79c76-108">I løbet af aftenen og i weekenden for regionen vil tjenesten dog være klar til at behandle en betydeligt større mængde anmodninger fra baggrundsapps.</span><span class="sxs-lookup"><span data-stu-id="79c76-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="79c76-109">**503-fejl ved overførsel til SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="79c76-109">**503 errors when migrating to SharePoint Online**</span></span>

<span data-ttu-id="79c76-110">Det ser ud til, at du overfører til SharePoint Online og modtager 503-fejl.</span><span class="sxs-lookup"><span data-stu-id="79c76-110">It appears you are migrating to SharePoint Online and receiving 503 errors.</span></span> <span data-ttu-id="79c76-111">Følg nedenstående trin, så vi kan hjælpe dig så hurtigt som muligt.</span><span class="sxs-lookup"><span data-stu-id="79c76-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="79c76-112">Klik på **Kontakt support**, og klik derefter på **Ny serviceanmodning**.</span><span class="sxs-lookup"><span data-stu-id="79c76-112">Click **Contact Support**, and then **New Service Request**.</span></span>
2. <span data-ttu-id="79c76-113">Skriv **SharePoint-begrænsning af overflytning med 503**for titlen og beskrivelsen.</span><span class="sxs-lookup"><span data-stu-id="79c76-113">For the title and description, type **SharePoint Migration Throttling with 503**.</span></span>
3. <span data-ttu-id="79c76-114">Når billetten er indsendt, skal du opdatere den med følgende oplysninger:</span><span class="sxs-lookup"><span data-stu-id="79c76-114">Once the ticket has been submitted, please update it with the following information:</span></span>
    - <span data-ttu-id="79c76-115">Hvor meget tilbage af migration (for eksempel, hvor mange TBs?).</span><span class="sxs-lookup"><span data-stu-id="79c76-115">How much left of migration (for example, how many TBs?).</span></span>
    - <span data-ttu-id="79c76-116">Start- og slutdato for overførsel.</span><span class="sxs-lookup"><span data-stu-id="79c76-116">Migration start and end date.</span></span>
    - <span data-ttu-id="79c76-117">Beskriv, hvor du overfører dit indhold fra, f.eks.</span><span class="sxs-lookup"><span data-stu-id="79c76-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>
    - <span data-ttu-id="79c76-118">Anslå antallet af begrænsningsfejl (f.eks. x gashåndtag pr. time?), og hvornår opstod begrænsningen.</span><span class="sxs-lookup"><span data-stu-id="79c76-118">Estimate the number of throttling errors (for example, x throttle per hour?) and when did the throttling happen.</span></span>
    - <span data-ttu-id="79c76-119">Hvilket overførselsværktøj du bruger (f.eks.</span><span class="sxs-lookup"><span data-stu-id="79c76-119">Which migration tool you are using (for example, SPMT or ShareGate).</span></span>


