---
title: 2419--til-Aktiver-overvågning
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 3af01c03711eed646f0009afb5bea685bc358196
ms.sourcegitcommit: 87153fec6f6468b57893abf4aac073ba4068e67b
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/19/2019
ms.locfileid: "35065621"
---
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="13f38-102">Der kunne ikke aktivere samlet overvågning</span><span class="sxs-lookup"><span data-stu-id="13f38-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="13f38-103">Når du forsøger at aktivere samlet overvågning for organisationen Office 365, kan du modtager en lignende fejl følgende:</span><span class="sxs-lookup"><span data-stu-id="13f38-103">When you try to enable unified auditing for your Office 365 organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="13f38-104">Du kan løse dette problem ved at følge disse trin:</span><span class="sxs-lookup"><span data-stu-id="13f38-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="13f38-105">[Oprette forbindelse til Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="13f38-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="13f38-106">Kør følgende cmdlet:</span><span class="sxs-lookup"><span data-stu-id="13f38-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="13f38-107">Vente i 60 minutter til den tidligere indstilling kan træde i kraft.</span><span class="sxs-lookup"><span data-stu-id="13f38-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="13f38-108">Kør følgende kommando i Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="13f38-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="13f38-109">Yderligere oplysninger finder du i følgende artikler:</span><span class="sxs-lookup"><span data-stu-id="13f38-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="13f38-110">Oprette forbindelse til Exchange Online PowerShell ved hjælp af godkendelse i flere niveauer</span><span class="sxs-lookup"><span data-stu-id="13f38-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="13f38-111">Slå Office 365 overvågning log søgning til eller fra</span><span class="sxs-lookup"><span data-stu-id="13f38-111">Turn Office 365 audit log search on or off</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
