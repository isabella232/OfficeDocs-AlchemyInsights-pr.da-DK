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
# <a name="unable-to-enable-unified-auditing"></a>Der kan ikke aktiveres en ensartet overvågning

NÃ¥r du forsÃ ̧ger at aktivere samlet overvågning for organisationen, kan du fÃ¥ vist en fejlmeddelelse, der ligner fÃ ̧lgende:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Du kan lÃ ̧se problemet ved at fÃ ̧lge disse trin:

1. [Opret forbindelse til Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Kør følgende cmdlet:

   ```
   Enable-OrganizationCustomization
   ```

3. Vent i 60 minutter, før den forrige indstilling træder i kraft.

4. Kør følgende kommando i Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Yderligere oplysninger finder du i følgende artikler:

- [Oprette forbindelse til Exchange Online PowerShell ved hjælp af multifaktorgodkendelse](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Slå søgning i overvågningsloggen til eller fra](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
