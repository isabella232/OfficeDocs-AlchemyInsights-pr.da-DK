---
title: Konfigurer indstillinger for beskyttelse af personlige oplysninger i Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 2367a7a55d1837fa7c7095fd0ac10ff1cf7ae72d
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404620"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a><span data-ttu-id="38c51-102">Konfigurer indstillinger for beskyttelse af personlige oplysninger i Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="38c51-102">Configure privacy settings in Microsoft Edge</span></span>

<span data-ttu-id="38c51-103">Hvis Microsoft Edge er installeret på ikke-Windows-platforme, sendes diagnostiske data og webstedsoplysninger som standard ikke til Microsoft.</span><span class="sxs-lookup"><span data-stu-id="38c51-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information aren't sent to Microsoft.</span></span> <span data-ttu-id="38c51-104">Men hvis Microsoft Edge er installeret på Windows 10, sendes diagnostiske data og webstedsoplysninger i overensstemmelse med brugernes indstillinger for [Diagnostiske Windows-data.](https://go.microsoft.com/fwlink/?linkid=2132472)</span><span class="sxs-lookup"><span data-stu-id="38c51-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://go.microsoft.com/fwlink/?linkid=2132472).</span></span>

<span data-ttu-id="38c51-105">Hvis du vil konfigurere, hvordan Microsoft Edge håndterer dataindsamling for din organisation, skal du bruge følgende gruppepolitikker:</span><span class="sxs-lookup"><span data-stu-id="38c51-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="38c51-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) aktiverer rapportering af brugs- og nedbrudsrelaterede data.</span><span class="sxs-lookup"><span data-stu-id="38c51-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) turns on reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="38c51-107">[SendSiteInfoToImproveServices sender webstedsoplysninger,](https://go.microsoft.com/fwlink/?linkid=2132470) der bruges til at forbedre Microsoft-tjenester.</span><span class="sxs-lookup"><span data-stu-id="38c51-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) sends site information used to improve Microsoft services.</span></span>

<span data-ttu-id="38c51-108">Du kan få mere at vide under [Konfigurer politikindstillinger.](https://go.microsoft.com/fwlink/?linkid=2132577)</span><span class="sxs-lookup"><span data-stu-id="38c51-108">To learn more, see [Configure policy settings](https://go.microsoft.com/fwlink/?linkid=2132577).</span></span>
