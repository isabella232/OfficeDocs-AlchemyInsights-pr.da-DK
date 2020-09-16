---
title: Fejlfinding af ydeevnen i OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 4699f6113acd70b4778f9feeaeec012ff8fdd63f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757879"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="76739-102">Fejlfinding af ydeevnen i OneDrive</span><span class="sxs-lookup"><span data-stu-id="76739-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="76739-103">Hvis du oplever en langsommere end forventet synkronisering eller lignende problemer med ydeevnen med OneDrive:</span><span class="sxs-lookup"><span data-stu-id="76739-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="76739-104">Bekræft, at der ikke er nogen kendte problemer ved hjælp af [dashboardet for tjenestetilstand](https://portal.office.com/adminportal/home?ref=/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="76739-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="76739-105">[Aktivér filer efter behov](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) , så du kan få adgang til alle dine filer i OneDrive uden at skulle downloade dem og bruge lagerplads på din enhed.</span><span class="sxs-lookup"><span data-stu-id="76739-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="76739-106">[Gennemgå de bedste fremgangsmåder](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for netværks planlægning og ydeevne.</span><span class="sxs-lookup"><span data-stu-id="76739-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="76739-107">[Maksimer overførsels-og downloadhastighed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), især hvis du synkroniserer en enhed for første gang.</span><span class="sxs-lookup"><span data-stu-id="76739-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="76739-108">Hvis du synkroniserer et bibliotek med mere end 100.000 elementer, kan OneDrive-synkronisering virke fast i et langt tidspunkt, eller status viser behandlings 0KB for xMB.</span><span class="sxs-lookup"><span data-stu-id="76739-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="76739-109">[Få mere at vide om at synkronisere mere end 100.000-filer](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) såvel som [onedrives understøttede grænse på 300.000-filer](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span><span class="sxs-lookup"><span data-stu-id="76739-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="76739-110">Når en bruger overskrider brugs begrænsningerne, begrænser SharePoint Online eventuelle yderligere anmodninger fra den pågældende brugerkonto i en kort periode.</span><span class="sxs-lookup"><span data-stu-id="76739-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="76739-111">Alle brugerhandlinger er begrænset, mens begrænsningen er aktiv.</span><span class="sxs-lookup"><span data-stu-id="76739-111">All user actions are throttled while the throttle is in effect.</span></span>
