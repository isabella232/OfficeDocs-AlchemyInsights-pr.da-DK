---
title: 2419-kan-ikke-aktivere-revision
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 23ad07a6dd943d61d1bd45453089a771cfd51b58
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510422"
---
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="3ef1b-102">Der kan ikke aktiveres en ensartet overvågning</span><span class="sxs-lookup"><span data-stu-id="3ef1b-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="3ef1b-103">NÃ¥r du forsÃ ̧ger at aktivere samlet overvågning for organisationen, kan du fÃ¥ vist en fejlmeddelelse, der ligner fÃ ̧lgende:</span><span class="sxs-lookup"><span data-stu-id="3ef1b-103">When you try to enable unified auditing for your organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="3ef1b-104">Du kan lÃ ̧se problemet ved at fÃ ̧lge disse trin:</span><span class="sxs-lookup"><span data-stu-id="3ef1b-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="3ef1b-105">[Opret forbindelse til Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="3ef1b-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="3ef1b-106">Kør følgende cmdlet:</span><span class="sxs-lookup"><span data-stu-id="3ef1b-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="3ef1b-107">Vent i 60 minutter, før den forrige indstilling træder i kraft.</span><span class="sxs-lookup"><span data-stu-id="3ef1b-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="3ef1b-108">Kør følgende kommando i Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="3ef1b-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="3ef1b-109">Yderligere oplysninger finder du i følgende artikler:</span><span class="sxs-lookup"><span data-stu-id="3ef1b-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="3ef1b-110">Oprette forbindelse til Exchange Online PowerShell ved hjælp af multifaktorgodkendelse</span><span class="sxs-lookup"><span data-stu-id="3ef1b-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="3ef1b-111">Slå søgning i overvågningsloggen til eller fra</span><span class="sxs-lookup"><span data-stu-id="3ef1b-111">Turn audit log search on or off</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
