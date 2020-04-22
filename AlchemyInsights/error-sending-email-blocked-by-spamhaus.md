---
title: Fejl under afsendelse af e-mail blokeret af SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714252"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="6b970-102">Fejl under afsendelse af mail: Klientvært blokeret ved hjælp af Spamhaus</span><span class="sxs-lookup"><span data-stu-id="6b970-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="6b970-103">Den IP-adresse, der sendte meddelelsen, findes på en blokeringsliste, der ejes af [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="6b970-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="6b970-104">Årsagerne til at blive blokeret af Spamhaus omfatter kompromitterede konti, kompromitterede maskiner, der deler en offentlig IP-adresse, og politikker for internetudbydere.</span><span class="sxs-lookup"><span data-stu-id="6b970-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="6b970-105">Mulige rettelser er:</span><span class="sxs-lookup"><span data-stu-id="6b970-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="6b970-106">For blokerede indgående meddelelser, hvor du styrer kildemailserveren, skal du finde årsagen og fjerne blokeringen fra Spamhaus's websted.</span><span class="sxs-lookup"><span data-stu-id="6b970-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="6b970-107">For blokerede indgående meddelelser, hvor kildens IP-adresse tilhører en anden, skal adresseejeren fjerne blokeringen fra Spamhaus's websted.</span><span class="sxs-lookup"><span data-stu-id="6b970-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="6b970-108">Hvis IP-adressen er på PBL (Policy Block List), kan ejeren tildele en anden statisk IP-adresse eller fjerne adressen fra PBL'en.</span><span class="sxs-lookup"><span data-stu-id="6b970-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="6b970-109">For blokerede udgående meddelelser fra dit domæne, der er tilsluttet Microsoft, kan du få vist denne fejl, hvis meddelelserne dirigeres via en tredjepartstjeneste.</span><span class="sxs-lookup"><span data-stu-id="6b970-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="6b970-110">Du kan bruge et WHOIS-opslagsværktøj til at finde den blokerede ip-adresseejer.</span><span class="sxs-lookup"><span data-stu-id="6b970-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
