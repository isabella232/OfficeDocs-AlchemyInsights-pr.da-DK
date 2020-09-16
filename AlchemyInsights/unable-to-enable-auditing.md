---
title: 2419 – kan ikke aktiveres-overvågning
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 81fd8e33feb2f2b10b04cc7cdc746a8603aa366b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767593"
---
# <a name="unable-to-enable-unified-auditing"></a>Det er ikke muligt at aktivere Unified revisions

Når du forsøger at aktivere Unified revisions for din organisation, får du muligvis en fejl, der ligner følgende:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Du kan løse dette problem ved at følge disse trin:

1. [Opret forbindelse til Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Kør følgende cmdlet:

   ```
   Enable-OrganizationCustomization
   ```

3. Vent på 60 minutter, til den forrige indstilling træder i kraft.

4. Kør følgende kommando i Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Du kan finde flere oplysninger i følgende artikler:

- [Opret forbindelse til Exchange Online PowerShell ved hjælp af multifaktorgodkendelse](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Slå søgning i overvågningsloggen til eller fra](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
