---
title: Fejlfinding i forbindelse med OneDrive-ydeevne
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 197a84c5f69f9e58460925049345263743fe78ee
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43733192"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="8df34-102">Fejlfinding i forbindelse med OneDrive-ydeevne</span><span class="sxs-lookup"><span data-stu-id="8df34-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="8df34-103">Hvis du oplever en langsommere synkronisering end forventet eller lignende problemer med ydeevnen med OneDrive:</span><span class="sxs-lookup"><span data-stu-id="8df34-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="8df34-104">Bekræft, at der ikke er nogen kendte problemer ved hjælp af [Dashboard for tjenestetilstand](https://portal.office.com/adminportal/home?ref=/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="8df34-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="8df34-105">[Aktivér Filer efter behov,](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) så du kan få adgang til alle dine filer i OneDrive uden at skulle hente dem alle og bruge lagerplads på din enhed.</span><span class="sxs-lookup"><span data-stu-id="8df34-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="8df34-106">[Gennemgå de bedste fremgangsmåder](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for netværksplanlægning og -ydeevne.</span><span class="sxs-lookup"><span data-stu-id="8df34-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="8df34-107">[Maksimer overførsels- og overførselshastigheden](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), især hvis du synkroniserer en enhed for første gang.</span><span class="sxs-lookup"><span data-stu-id="8df34-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="8df34-108">Hvis du synkroniserer et bibliotek med mere end 100.000 elementer, kan OneDrive-synkronisering virke fast i lang tid, eller status viser Behandling af 0 KB xMB."</span><span class="sxs-lookup"><span data-stu-id="8df34-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="8df34-109">Få mere at vide om synkronisering af [mere end 100.000 filer](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) samt [OneDrive's understøttede grænse på 300.000 filer](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span><span class="sxs-lookup"><span data-stu-id="8df34-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="8df34-110">Når en bruger overskrider brugsgrænserne, begrænser SharePoint Online yderligere anmodninger fra den pågældende brugerkonto i en kort periode.</span><span class="sxs-lookup"><span data-stu-id="8df34-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="8df34-111">Alle brugerhandlinger begrænses, mens gashåndtaget er aktiveret.</span><span class="sxs-lookup"><span data-stu-id="8df34-111">All user actions are throttled while the throttle is in effect.</span></span>
