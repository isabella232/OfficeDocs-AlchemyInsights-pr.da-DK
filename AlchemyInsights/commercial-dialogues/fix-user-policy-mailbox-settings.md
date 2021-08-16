---
title: Ret indstillinger for brugerpolitik/postkasse
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: fecc52bea66e0aed709a8995d2509f4432c09482459aa575d29e4c7551375211
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034712"
---
# <a name="fix-user-policymailbox-settings"></a>Ret indstillinger for brugerpolitik/postkasse

Indstillingerne for uønsket mail på postkassen påvirkede denne meddelelse. Hvis du vil gennemse indstillingerne, skal du gøre følgende:

1. Start Exchange Management Shell. Du kan få mere at [vide under Åbn Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
2. Kør denne kommando (ved hjælp af brugerens mailadresse):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Kontrollér, om afsenderens mailadresse er en del af **TrustedSendersAndDomains** eller **BlockedSendersAndDomains.** Hvis mailadressen er på en af listerne, skal du muligvis fjerne den. Du kan få mere at [vide under Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).
