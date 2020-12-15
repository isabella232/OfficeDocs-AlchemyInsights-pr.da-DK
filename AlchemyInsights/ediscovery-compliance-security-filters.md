---
title: Ingen resultater returneret under indholdssøgning/eksport
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/14/2020
ms.locfileid: "49677681"
---
# <a name="no-results-returned-during-content-searchexport"></a><span data-ttu-id="24dc3-102">Ingen resultater returneret under indholdssøgning/eksport</span><span class="sxs-lookup"><span data-stu-id="24dc3-102">No results returned during Content Search/Export</span></span>

<span data-ttu-id="24dc3-103">Hvis du oplever problemer med følgende eDiscovery-scenarier:</span><span class="sxs-lookup"><span data-stu-id="24dc3-103">If you are experiencing issues with the following eDiscovery scenarios:</span></span>

- <span data-ttu-id="24dc3-104">Indholdssøgning/eksport returnerer ingen data eller uventede data</span><span class="sxs-lookup"><span data-stu-id="24dc3-104">Content Search/Export returns no data or unexpected data</span></span>
- <span data-ttu-id="24dc3-105">eDiscovery-søgning eller eksport mislykkes</span><span class="sxs-lookup"><span data-stu-id="24dc3-105">eDiscovery Search or Export fails</span></span>

<span data-ttu-id="24dc3-106">Dette kan skyldes visse sikkerhedsfiltre for overholdelse, der blev oprettet af en bestemt administrator, og som ikke er blevet kommunikeret med alle administratorer.</span><span class="sxs-lookup"><span data-stu-id="24dc3-106">This may be caused due to certain Compliance Security Filters that were setup by a specific Admin and not been communicated to all Admins.</span></span>

<span data-ttu-id="24dc3-107">Hvis du vil løse dette, skal du kontrollere, om der er nogen sikkerhedsfiltre for overholdelse, der kan forårsage disse problemer:</span><span class="sxs-lookup"><span data-stu-id="24dc3-107">To resolve this, check if there are any Compliance Security Filters that may be causing these issues:</span></span>

1. <span data-ttu-id="24dc3-108">Opret forbindelse til sikkerheds-og overholdelses Center PowerShell</span><span class="sxs-lookup"><span data-stu-id="24dc3-108">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="24dc3-109">Kør følgende commandlets:</span><span class="sxs-lookup"><span data-stu-id="24dc3-109">Run the following commandlets:</span></span>

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

<span data-ttu-id="24dc3-110">Du kan finde flere oplysninger om kompatibilitets relaterede filtre under [tilladelser til filtrering af indholdssøgning](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span><span class="sxs-lookup"><span data-stu-id="24dc3-110">For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span></span>
