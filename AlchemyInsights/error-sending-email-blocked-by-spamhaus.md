---
title: Fejl under afsendelse af mail, der er blokeret af spam Haus
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783797"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="fcd65-102">Fejl ved afsendelse af mail: klient vært blokeret ved hjælp af spam Haus</span><span class="sxs-lookup"><span data-stu-id="fcd65-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="fcd65-103">Den IP-adresse, der sendte meddelelsen, er på en blokliste, der ejes af [spam Haus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="fcd65-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="fcd65-104">Grunde til at blive blokeret af spam Haus omfatter skadede konti, kompromitterede maskiner, der deler en offentlig IP-adresse og en internetudbyder (ISP)-politikker.</span><span class="sxs-lookup"><span data-stu-id="fcd65-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="fcd65-105">Mulige rettelser:</span><span class="sxs-lookup"><span data-stu-id="fcd65-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="fcd65-106">For blokerede indgående meddelelser, hvor du styrer kilde mailserveren, skal du finde årsagen og fjerne blokken fra spam Haus websted.</span><span class="sxs-lookup"><span data-stu-id="fcd65-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="fcd65-107">For blokerede indgående meddelelser, hvor kildens IP-adresse tilhører en anden, skal adresse ejeren fjerne blokken fra spam Haus websted.</span><span class="sxs-lookup"><span data-stu-id="fcd65-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="fcd65-108">Hvis IP-adressen er på listen politik blok (PBL), kan ejeren tildele en anden statisk IP-adresse eller fjerne adressen fra PBL.</span><span class="sxs-lookup"><span data-stu-id="fcd65-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="fcd65-109">For blokerede udgående meddelelser fra dit domæne, der er knyttet til Microsoft, kan du få denne fejl, hvis meddelelserne sendes via en tredjepartstjeneste.</span><span class="sxs-lookup"><span data-stu-id="fcd65-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="fcd65-110">Du kan bruge et WHOIS-opslagsværktøj til at finde den blokerede IP-adresse ejer.</span><span class="sxs-lookup"><span data-stu-id="fcd65-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
