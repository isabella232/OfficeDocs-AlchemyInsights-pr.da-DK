---
title: Indholdssøgning uden resultater
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680641"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="a73c9-102">Ingen resultater fra indholdssøgning/eksport</span><span class="sxs-lookup"><span data-stu-id="a73c9-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="a73c9-103">Problemer med indholdssøgning/eksport, der ikke returnerer nogen data, kan skyldes et bestemt sikkerheds filter for overholdelse, der blev konfigureret af en bestemt administrator og ikke kommunikerer med alle administratorer.</span><span class="sxs-lookup"><span data-stu-id="a73c9-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="a73c9-104">Hvis du vil løse dette, skal du kontrollere, om der er nogen sikkerhedsfiltre overholdelse, der kan forårsage dette:</span><span class="sxs-lookup"><span data-stu-id="a73c9-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="a73c9-105">Opret forbindelse til sikkerheds-og overholdelses Center PowerShell</span><span class="sxs-lookup"><span data-stu-id="a73c9-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="a73c9-106">Kør følgende commandlets:</span><span class="sxs-lookup"><span data-stu-id="a73c9-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="a73c9-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="a73c9-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="a73c9-108">Få ComplianceSecurityFilter-organisation $org</span><span class="sxs-lookup"><span data-stu-id="a73c9-108">Get-ComplianceSecurityFilter -Organization $org</span></span>