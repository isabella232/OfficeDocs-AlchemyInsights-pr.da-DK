---
title: Indhold søgeresultater ikke
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800266"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="6bfc1-102">Ingen resultater fra indhold Søg/eksport</span><span class="sxs-lookup"><span data-stu-id="6bfc1-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="6bfc1-103">Problemer med indhold Søg/eksport ikke returnere data, kan skyldes, at visse overholdelse sikkerhedsfilter, der var opsætning ved en bestemt Admin og kommunikerer ikke til alle administratorer.</span><span class="sxs-lookup"><span data-stu-id="6bfc1-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="6bfc1-104">Du kan løse dette ved at kontrollere for at se, om der er nogen overensstemmelse sikkerhedsfiltre, som kan forårsage dette:</span><span class="sxs-lookup"><span data-stu-id="6bfc1-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="6bfc1-105">Oprette forbindelse til sikkerhed og Overholdelsescenter Powershell</span><span class="sxs-lookup"><span data-stu-id="6bfc1-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="6bfc1-106">Kør følgende cmdlet'er:</span><span class="sxs-lookup"><span data-stu-id="6bfc1-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="6bfc1-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="6bfc1-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="6bfc1-108">Get-ComplianceSecurityFilter-organisation $org</span><span class="sxs-lookup"><span data-stu-id="6bfc1-108">Get-ComplianceSecurityFilter -Organization $org</span></span>