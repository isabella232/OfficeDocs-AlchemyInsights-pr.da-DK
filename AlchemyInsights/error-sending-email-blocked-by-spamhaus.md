---
title: Fejl under afsendelse af e-mail, der er blokeret af SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 52a5c20d59a2eac4c4bf465edaa888952d47f39f
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/28/2019
ms.locfileid: "35387843"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="206ca-102">Fejl under afsendelse af e-mail: klient-vært, der er blokeret ved hjælp af Spamhaus</span><span class="sxs-lookup"><span data-stu-id="206ca-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="206ca-103">Den IP-adresse, sendes meddelelsen er på en liste over blokerede websteder ejes af [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="206ca-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="206ca-104">Årsager til at blive blokeret af Spamhaus omfatter skadet konti skadet maskiner dele en offentlig IP-adresse og politikker for internetudbyder (ISP).</span><span class="sxs-lookup"><span data-stu-id="206ca-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="206ca-105">Mulige løsninger er:</span><span class="sxs-lookup"><span data-stu-id="206ca-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="206ca-106">Blokerede indgående meddelelser til Office 365, hvor du styrer e-mail-kildeserveren, skal du finde årsagen og fjerne blokeringen fra webstedet Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="206ca-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="206ca-107">Blokerede indgående meddelelser til Office 365, hvor kilde-IP-adresse hører til en anden, skal ejeren af adressen blokeringen fjernes fra webstedet Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="206ca-107">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="206ca-108">Hvis IP-adressen på politikken Block liste (PBL), kan ejeren tildele en anden statisk IP-adresse eller fjerne adressen fra PBL.</span><span class="sxs-lookup"><span data-stu-id="206ca-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="206ca-109">For blokerede udgående meddelelser fra dit domæne til Office 365, kan du modtager denne fejlmeddelelse, hvis meddelelser dirigeres gennem en 3. part service.</span><span class="sxs-lookup"><span data-stu-id="206ca-109">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="206ca-110">Du kan bruge et værktøj til opslag af WHO-IS til at finde ejeren af blokerede IP-adresse.</span><span class="sxs-lookup"><span data-stu-id="206ca-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
