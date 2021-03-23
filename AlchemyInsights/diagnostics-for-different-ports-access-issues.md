---
title: Diagnosticering af forskellige adgangsproblemer med porte
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035264"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Diagnosticering af forskellige adgangsproblemer med porte

Du kan løse de forskellige problemer med portadgang ved at udføre følgende trin:

1. Stop/dealloker den virtuelle maskine (VM) fra portalen, genstart VM'en, og test igen. 
2. Kontrollér din VM's netværksindstillinger for at finde ud af, om du har NSG'er (Network Security Groups), der blokerer trafik. Du kan også bruge [Network Watcher's](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) IP-flowkontrolværktøj til at kontrollere, om NSG'er blokerer trafik, User-Defined Routes(UDR) omrogerer din trafik tilbage til det lokale miljø (standardrute' 0.0.0.0/0) eller til et netværkskab.
Hvis du stadig oplever problemer efter at have forsøgt ovenstående trin, skal du angive navnet på VM og den TCP-port, du forsøger at sende mails på for at få diagnosticeret yderligere.

**Anbefalede dokumenter**

[Begrænsninger og anbefalinger til afsendelse af udgående mail over port 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)