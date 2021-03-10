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
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/09/2021
ms.locfileid: "50693305"
---
# <a name="fix-user-policymailbox-settings"></a>Ret indstillinger for brugerpolitik/postkasse

Indstillingerne for uønsket mail på postkassen påvirkede denne meddelelse. Hvis du vil gennemse indstillingerne, skal du gøre følgende:

1. Start Shell til Exchange-administration. Du kan finde flere oplysninger [i Åbn Shell til Exchange-administration.](https://go.microsoft.com/fwlink/?linkid=2101432)
2. Kør denne kommando (ved hjælp af brugerens mailadresse):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Kontrollér, om afsenderens mailadresse er en del af **TrustedSendersAndDomains** eller **BlockedSendersAndDomains.** Hvis mailadressen er på en af listerne, skal du muligvis fjerne den. Du kan få mere at [vide under Set-MailboxJunkEmailConfiguration.](https://go.microsoft.com/fwlink/?linkid=2101047)
