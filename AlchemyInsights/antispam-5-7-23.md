---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506437"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Løs problemer med levering af e-mail for fejlkode 5.7.23

Kontroller SPF DNS-posten for dit domæne ved en offentligt tilgængelig SPF- eller DNS-postkontrol på internettet.

Kontroller, at den udgående meddelelse ikke blev identificeret som spam af Microsoft og dirigeret gennem [high risk-leveringspuljen](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). Meddelelser i højrisikoleveringspuljen består ikke SPF-kontroller og accepteres derfor ikke af destinationsmailorganisationen.

Hvis problemet fortsætter, skal du muligvis kontakte administratoren af den mailvært, som du forsøger at sende e-mail til. Gør opmærksom på den detaljerede eksterne fejl, der er tilgængelig i afvisningsmeddelelsen. Microsoft-support kan muligvis ikke hjælpe yderligere.
