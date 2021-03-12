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
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a><span data-ttu-id="0e54b-102">Det er ikke muligt at sende/modtage mails til/fra Office 365 på grund af deaktivering af TLS 1.0 og TLS 1.1</span><span class="sxs-lookup"><span data-stu-id="0e54b-102">Unable to send/receive email to/from Office 365 because of the TLS 1.0 and TLS 1.1 disablement</span></span>

<span data-ttu-id="0e54b-103">Som bekræftet af meddelelsescenteret efter MC229914 begyndte udrådningen af TLS 1.0 og TLS 1.1 at gennemtvinge gennemtvingelse af slutpunkter for mailflow i Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="0e54b-103">As confirmed by the message center post MC229914, TLS 1.0 and TLS 1.1 deprecation started enforcing for Exchange Online mail flow endpoints.</span></span> <span data-ttu-id="0e54b-104">Office 365 accepterer snart ikke længere TLS 1.0- og TLS 1.1-mailforbindelser fra eksterne kilder.</span><span class="sxs-lookup"><span data-stu-id="0e54b-104">Soon Office 365 will no longer accept TLS 1.0 and TLS 1.1 email connections from external sources.</span></span> <span data-ttu-id="0e54b-105">Desuden bruger Exchange Online aldrig TLS 1.0 eller 1.1 til at sende udgående mail.</span><span class="sxs-lookup"><span data-stu-id="0e54b-105">Also, Exchange Online will never use TLS 1.0 or 1.1 to send outbound email.</span></span> <span data-ttu-id="0e54b-106">Hvis du oplever problemer på grund af deaktivering af TLS 1.0 eller 1.1, kan du opleve en af følgende fejl:</span><span class="sxs-lookup"><span data-stu-id="0e54b-106">If you are facing issues because of TLS 1.0 or 1.1 disablement, you might experience one of the following errors-</span></span>

- <span data-ttu-id="0e54b-107">Afsenderen får NDR tilbage – '421 4.4.2 Forbindelse tabt på grund af SocketError'</span><span class="sxs-lookup"><span data-stu-id="0e54b-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="0e54b-108">Fejl i køvisningen for den lokale server, der sender mail til Officer 365 – '421 4.4.2 Forbindelse tabt på grund af SocketError'</span><span class="sxs-lookup"><span data-stu-id="0e54b-108">Error in the Queue Viewer of On-Premises server that is sending email to Officer 365- '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="0e54b-109">Fejl i Send [forbindelsesprotokollog på](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) den server, der sender mail til Office 365 – TLS-aftalen mislykkedes med fejlen SocketError</span><span class="sxs-lookup"><span data-stu-id="0e54b-109">Error in Send connector [Protocol log](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) on the server sending email to Office 365- TLS negotiation failed with error SocketError</span></span>
- <span data-ttu-id="0e54b-110">Fejl i Send eller modtag forbindelsesprotokollog – '451 5.7.3 Skal først udstede en STARTTLS-kommando'</span><span class="sxs-lookup"><span data-stu-id="0e54b-110">Error in Send or receive connector protocol log - '451 5.7.3 Must issue a STARTTLS command first'</span></span>

<span data-ttu-id="0e54b-111">Hvis du oplever nogen af ovenstående fejl, skal du kontrollere, at den server, der sender eller modtager mails, har TLS 1.2 aktiveret ved at kontrollere følgende registreringsdatabasenøgler:</span><span class="sxs-lookup"><span data-stu-id="0e54b-111">If you experience any of the above errors, please make sure the server that is sending or receiving email has TLS 1.2 enabled by checking the following registry keys-</span></span>

<span data-ttu-id="0e54b-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2\Klient] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:000000001**</span><span class="sxs-lookup"><span data-stu-id="0e54b-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span></span>

<span data-ttu-id="0e54b-113">Hvis du foretager ændringer i ovenstående registreringsdatabasenøgler for at aktivere TLS 1.2, skal du genstarte serveren, før ændringerne træder i kraft.</span><span class="sxs-lookup"><span data-stu-id="0e54b-113">If you make any change in the above registry keys to enable TLS 1.2, restart the server for the changes to take effect.</span></span> <span data-ttu-id="0e54b-114">Sørg også for, at du har de nyeste Windows- og Exchange-opdateringer installeret.</span><span class="sxs-lookup"><span data-stu-id="0e54b-114">Also make sure you have the latest Windows and Exchange updates installed.</span></span>

<span data-ttu-id="0e54b-115">Du kan finde flere oplysninger under:</span><span class="sxs-lookup"><span data-stu-id="0e54b-115">For more information, see:</span></span>

- [<span data-ttu-id="0e54b-116">Exchange Server TLS-vejledning, del 1: Gør klar til TLS 1.2 – Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="0e54b-116">Exchange Server TLS guidance, part 1: Getting Ready for TLS 1.2 - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [<span data-ttu-id="0e54b-117">Exchange Server TLS-vejledning Del 2: Aktivering af TLS 1.2 og identifikation af klienter, der ikke bruger det – Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="0e54b-117">Exchange Server TLS guidance Part 2: Enabling TLS 1.2 and Identifying Clients Not Using It - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [<span data-ttu-id="0e54b-118">Forstå mailscenarier, hvis der ikke kan aftales TLS-versioner med Exchange Online – Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="0e54b-118">Understanding email scenarios if TLS versions cannot be agreed on with Exchange Online - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
