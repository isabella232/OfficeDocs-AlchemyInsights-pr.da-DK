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
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516773"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="f4423-102">Ingen resultater fra indhold Søg/eksport</span><span class="sxs-lookup"><span data-stu-id="f4423-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="f4423-103">Problemer med indhold Søg/eksport ikke returnere data, kan skyldes, at visse overholdelse sikkerhedsfilter, der var opsætning ved en bestemt Admin og kommunikerer ikke til alle administratorer.</span><span class="sxs-lookup"><span data-stu-id="f4423-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="f4423-104">Du kan løse dette ved at kontrollere for at se, om der er nogen overensstemmelse sikkerhedsfiltre, som kan forårsage dette:</span><span class="sxs-lookup"><span data-stu-id="f4423-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="f4423-105">Oprette forbindelse til sikkerhed og Overholdelsescenter Powershell</span><span class="sxs-lookup"><span data-stu-id="f4423-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="f4423-106">Kør følgende cmdlet'er:</span><span class="sxs-lookup"><span data-stu-id="f4423-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="f4423-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="f4423-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="f4423-108">Get-ComplianceSecurityFilter-organisation $org</span><span class="sxs-lookup"><span data-stu-id="f4423-108">Get-ComplianceSecurityFilter -Organization $org</span></span>