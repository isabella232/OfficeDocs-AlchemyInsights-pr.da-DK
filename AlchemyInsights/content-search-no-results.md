---
title: Indholdssøgning uden resultater
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816842"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="6b324-102">Ingen resultater fra indholdssøgning/eksporter</span><span class="sxs-lookup"><span data-stu-id="6b324-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="6b324-103">Problemer med indholdssøgning/eksporter, der ikke returnerer nogen data, kan skyldes et bestemt sikkerhedsfilter til overholdelse, der er konfigureret af en bestemt administrator og ikke kommunikerer det til alle administratorer.</span><span class="sxs-lookup"><span data-stu-id="6b324-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="6b324-104">For at løse dette skal du kontrollere, om der er nogen sikkerhedsfiltre til overholdelse af regler og standarder, der kan være skyld i dette:</span><span class="sxs-lookup"><span data-stu-id="6b324-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="6b324-105">Opret forbindelse til Security and Compliance Center Powershell</span><span class="sxs-lookup"><span data-stu-id="6b324-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="6b324-106">Kør følgende kommandoletter:</span><span class="sxs-lookup"><span data-stu-id="6b324-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="6b324-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="6b324-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="6b324-108">Get-ComplianceSecurityFilter – $org</span><span class="sxs-lookup"><span data-stu-id="6b324-108">Get-ComplianceSecurityFilter -Organization $org</span></span>