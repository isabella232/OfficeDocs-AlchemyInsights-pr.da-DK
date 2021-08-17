---
title: Det er ikke muligt at sende/modtage mails til/Office 365 på grund af deaktivering af TLS 1.0 og TLS 1.1
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
ms.openlocfilehash: 508e48fd0e46557de075f4752da017ab8cc326923a965350140e598f7f7cf557
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054900"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Det er ikke muligt at sende/modtage mails til/Office 365 på grund af deaktivering af TLS 1.0 og TLS 1.1

Som bekræftet af meddelelsescenteret efter MC229914 begyndte udrådningen af TLS 1.0 og TLS 1.1 for at gennemtvinge Exchange Online for mailflowslutpunkter. Snart Office 365 ikke længere acceptere TLS 1.0- og TLS 1.1-mailforbindelser fra eksterne kilder. Desuden vil Exchange Online aldrig bruge TLS 1.0 eller 1.1 til at sende udgående mail. Hvis du oplever problemer på grund af deaktivering af TLS 1.0 eller 1.1, kan du opleve en af følgende fejl:

- Afsenderen får NDR afvist – '421 4.4.2 Forbindelse tabt på grund af SocketError'
- Fejl i Køvisning på den lokale server, der sender mail til Officer 365- '421 4.4.2 Forbindelsen er tabt på grund af SocketError'
- Fejl i Send [forbindelsesprotokollog på](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) serveren, der sender mails Office 365- TLS-aftale mislykkedes med fejlen SocketError
- Fejl i logfilen Send eller modtag forbindelsesprotokol – '451 5.7.3 Skal først udstede en STARTTLS-kommando'

Hvis du oplever en af ovenstående fejl, skal du kontrollere, at den server, der sender eller modtager mail, har TLS 1.2 aktiveret ved at kontrollere følgende registreringsdatabasenøgler-

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2\Klient] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**

Hvis du foretager ændringer i ovenstående registreringsdatabasenøgler for at aktivere TLS 1.2, skal du genstarte serveren, før ændringerne træder i kraft. Sørg også for, at du har de nyeste Windows og Exchange opdateringer installeret.

Du kan finde flere oplysninger under:

- [Exchange Server TLS-vejledning, del 1: Gør klar til TLS 1.2 – Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Server TLS-vejledning Del 2: Aktivering af TLS 1.2 og identificering af klienter, der ikke bruger det – Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Forstå mailscenarier, hvis der ikke kan aftales TLS-versioner med Exchange Online – Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
