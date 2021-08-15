---
title: Diagnosticering af problemer med adgang til forskellige porte
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
ms.openlocfilehash: 07c108d5292965d20340da039b67744d93c0a4fc61edb8115796671f2f7f1552
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030896"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Diagnosticering af problemer med adgang til forskellige porte

Du kan løse de forskellige problemer med portadgang ved at udføre følgende trin:

1. Stop/dealloker den virtuelle maskine (VM) fra portalen, genstart VM'en, og test igen. 
2. Kontrollér DIN VM's netværksindstillinger for at finde ud af, om du har NSG'er (Network Security Groups), der blokerer trafik. Du kan også bruge IP-flowkontrolværktøjet i [Network Watchers IP-flow](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) til at kontrollere, om NSG'er blokerer for trafik, User-Defined Ruter (UDR'er), der sender din trafik tilbage til et lokalt miljø ('Standardrute' 0.0.0/0) eller til et netværkspil.
Hvis du stadig oplever problemer efter at have prøvet ovenstående trin, skal du angive VM-navnet og den TCP-port, du forsøger at sende mail på for at få diagnosticeret yderligere.

**Anbefalede dokumenter**

[Begrænsninger og anbefalinger til at sende udgående mail over port 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)