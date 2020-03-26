---
title: Overførsel til SharePoint Online via Overførselsstyring
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
- "3192"
ms.openlocfilehash: 5aebf7903670e74f616c8f151749d760caf1d642
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931970"
---
# <a name="migrating-to-sharepoint-online-via-migration-manager"></a><span data-ttu-id="9fe6b-102">Overførsel til SharePoint Online via Overførselsstyring</span><span class="sxs-lookup"><span data-stu-id="9fe6b-102">Migrating to SharePoint Online via Migration Manager</span></span>

<span data-ttu-id="9fe6b-103">**Vigtigt**: Mange SharePoint Online- og OneDrive-kunder kører forretningskritiske programmer op mod tjenesten, der kører i baggrunden.</span><span class="sxs-lookup"><span data-stu-id="9fe6b-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="9fe6b-104">Disse omfatter indholdsoverførsel, forebyggelse af datatab (DLP) og løsninger til sikkerhedskopiering.</span><span class="sxs-lookup"><span data-stu-id="9fe6b-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="9fe6b-105">I disse hidtil usete tider tager vi skridt til at sikre, at SharePoint Online- og OneDrive-tjenester forbliver meget tilgængelige og pålidelige for dine brugere, der er mere afhængige af din tjeneste end nogensinde før i fjernarbejdssituationer.</span><span class="sxs-lookup"><span data-stu-id="9fe6b-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="9fe6b-106">For at understøtte denne målsætning har vi implementeret strengere begrænsninger for baggrundsapps (overførsel, DLP og løsninger til sikkerhedskopiering) i dagtimerne på hverdage.</span><span class="sxs-lookup"><span data-stu-id="9fe6b-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="9fe6b-107">Du bør forvente, at disse apps vil opnå en meget begrænset dataoverførselshastighed i disse tidsrum.</span><span class="sxs-lookup"><span data-stu-id="9fe6b-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="9fe6b-108">Derimod vil tjenesten i løbet af aften- og weekendtimerne i dit område være klar til at behandle en betydeligt højere mængde forespørgsler fra baggrundsapps.</span><span class="sxs-lookup"><span data-stu-id="9fe6b-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="9fe6b-109">**Overførselsstyring**</span><span class="sxs-lookup"><span data-stu-id="9fe6b-109">**Migration Manager**</span></span>

<span data-ttu-id="9fe6b-110">Overførselsstyring findes i det moderne SharePoint Administrationscenter og guider dig gennem opsætningen af dine klienter og oprettelse af dine opgaver.</span><span class="sxs-lookup"><span data-stu-id="9fe6b-110">Located in the modern SharePoint Admin Center, the Migration Manager guides you through the setup of your clients and the creation of your tasks.</span></span> <span data-ttu-id="9fe6b-111">Du kan angive globale indstillinger eller indstillinger på opgaveniveau, få vist opgavestatus og downloade aggregerede oplysninger og rapporter på opgaveniveau.</span><span class="sxs-lookup"><span data-stu-id="9fe6b-111">You can specify global or task-level settings, view all-up task progress, and download aggregated summary and task-level reports.</span></span>

- [<span data-ttu-id="9fe6b-112">Introduktion til Overførselsstyring</span><span class="sxs-lookup"><span data-stu-id="9fe6b-112">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="9fe6b-113">Konfiguration af klienter til Overførselsstyring</span><span class="sxs-lookup"><span data-stu-id="9fe6b-113">Setup Migration Manager clients</span></span>](https://docs.microsoft.com/sharepointmigration/mm-setup-clients)

- [<span data-ttu-id="9fe6b-114">Indstillinger for Overførselsstyring</span><span class="sxs-lookup"><span data-stu-id="9fe6b-114">Migration Manager Settings</span></span>](https://docs.microsoft.com/sharepointmigration/mm-settings)
