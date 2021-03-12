---
title: Det er ikke muligt at sende/modtage mails til/fra Office 365 på grund af deaktivering af TLS 1.0 og TLS 1.1
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743971"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Det er ikke muligt at sende/modtage mails til/fra Office 365 på grund af deaktivering af TLS 1.0 og TLS 1.1

Som bekræftet af meddelelsescenteret efter MC229914 begyndte udrådningen af TLS 1.0 og TLS 1.1 at gennemtvinge gennemtvingelse af slutpunkter for mailflow i Exchange Online. Office 365 accepterer snart ikke længere TLS 1.0- og TLS 1.1-mailforbindelser fra eksterne kilder. Desuden bruger Exchange Online aldrig TLS 1.0 eller 1.1 til at sende udgående mail. Hvis du oplever problemer på grund af deaktivering af TLS 1.0 eller 1.1, kan du opleve en af følgende fejl:

- Afsenderen får NDR tilbage – '421 4.4.2 Forbindelse tabt på grund af SocketError'
- Fejl i køvisningen for den lokale server, der sender mail til Officer 365 – '421 4.4.2 Forbindelse tabt på grund af SocketError'
- Fejl i Send [forbindelsesprotokollog på](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) den server, der sender mail til Office 365 – TLS-aftalen mislykkedes med fejlen SocketError
- Fejl i Send eller modtag forbindelsesprotokollog – '451 5.7.3 Skal først udstede en STARTTLS-kommando'

Hvis du oplever nogen af ovenstående fejl, skal du kontrollere, at den server, der sender eller modtager mails, har TLS 1.2 aktiveret ved at kontrollere følgende registreringsdatabasenøgler:

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2\Klient] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:000000001**

Hvis du foretager ændringer i ovenstående registreringsdatabasenøgler for at aktivere TLS 1.2, skal du genstarte serveren, før ændringerne træder i kraft. Sørg også for, at du har de nyeste Windows- og Exchange-opdateringer installeret.

Du kan finde flere oplysninger under:

- [Exchange Server TLS-vejledning, del 1: Gør klar til TLS 1.2 – Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Server TLS-vejledning Del 2: Aktivering af TLS 1.2 og identifikation af klienter, der ikke bruger det – Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Forstå mailscenarier, hvis der ikke kan aftales TLS-versioner med Exchange Online – Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
