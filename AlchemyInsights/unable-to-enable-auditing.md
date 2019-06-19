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
# <a name="unable-to-enable-unified-auditing"></a>Der kunne ikke aktivere samlet overvågning

Når du forsøger at aktivere samlet overvågning for organisationen Office 365, kan du modtager en lignende fejl følgende:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Du kan løse dette problem ved at følge disse trin:

1. [Oprette forbindelse til Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Kør følgende cmdlet:

   ```
   Enable-OrganizationCustomization
   ```

3. Vente i 60 minutter til den tidligere indstilling kan træde i kraft.

4. Kør følgende kommando i Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Yderligere oplysninger finder du i følgende artikler:

- [Oprette forbindelse til Exchange Online PowerShell ved hjælp af godkendelse i flere niveauer](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Slå Office 365 overvågning log søgning til eller fra](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
