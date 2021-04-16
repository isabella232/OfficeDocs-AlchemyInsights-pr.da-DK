---
title: Fejl under afsendelse af mails blokeret af SpamHaus
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813718"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="a0e6c-102">Fejl under afsendelse af mail: Klientvært blokeret ved hjælp af Spamhaus</span><span class="sxs-lookup"><span data-stu-id="a0e6c-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="a0e6c-103">IP-adressen, der sendte meddelelsen, er på en liste over blokerede afsendere, der ejes [af Spamhaus.](https://go.microsoft.com/fwlink/p/?linkid=123245)</span><span class="sxs-lookup"><span data-stu-id="a0e6c-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="a0e6c-104">Grunde til at blive blokeret af Spamhaus omfatter kompromitterede konti, kompromitterede computere, deling af en offentlig IP-adresse og politikker for internetudbydere.</span><span class="sxs-lookup"><span data-stu-id="a0e6c-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="a0e6c-105">De mulige rettelser er:</span><span class="sxs-lookup"><span data-stu-id="a0e6c-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="a0e6c-106">For blokerede indgående meddelelser, hvor du styrer kildemailserveren, skal du bestemme årsagen og fjerne blokeringen fra Spamhaus-webstedet.</span><span class="sxs-lookup"><span data-stu-id="a0e6c-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="a0e6c-107">For blokerede indgående meddelelser, hvor kilde-IP-adressen tilhører en anden, skal adressens ejer fjerne blokeringen fra Spamhaus-webstedet.</span><span class="sxs-lookup"><span data-stu-id="a0e6c-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="a0e6c-108">Hvis IP-adressen er på listen over blokerede politikker (Policy Block List – PBL), kan ejeren tildele en anden statisk IP-adresse eller fjerne adressen fra PBL.</span><span class="sxs-lookup"><span data-stu-id="a0e6c-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="a0e6c-109">For blokerede udgående meddelelser fra dit domæne, der er forbundet til Microsoft, kan du få vist denne fejl, hvis meddelelserne sendes via en tredjepartstjeneste.</span><span class="sxs-lookup"><span data-stu-id="a0e6c-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="a0e6c-110">Du kan bruge et WHOIS-opslagsværktøj til at finde ejeren af den blokerede IP-adresse.</span><span class="sxs-lookup"><span data-stu-id="a0e6c-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
