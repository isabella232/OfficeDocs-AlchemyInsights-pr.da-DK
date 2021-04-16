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
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Fejl under afsendelse af mail: Klientvært blokeret ved hjælp af Spamhaus

IP-adressen, der sendte meddelelsen, er på en liste over blokerede afsendere, der ejes [af Spamhaus.](https://go.microsoft.com/fwlink/p/?linkid=123245) Grunde til at blive blokeret af Spamhaus omfatter kompromitterede konti, kompromitterede computere, deling af en offentlig IP-adresse og politikker for internetudbydere. De mulige rettelser er:
  
- For blokerede indgående meddelelser, hvor du styrer kildemailserveren, skal du bestemme årsagen og fjerne blokeringen fra Spamhaus-webstedet.

- For blokerede indgående meddelelser, hvor kilde-IP-adressen tilhører en anden, skal adressens ejer fjerne blokeringen fra Spamhaus-webstedet. Hvis IP-adressen er på listen over blokerede politikker (Policy Block List – PBL), kan ejeren tildele en anden statisk IP-adresse eller fjerne adressen fra PBL.

- For blokerede udgående meddelelser fra dit domæne, der er forbundet til Microsoft, kan du få vist denne fejl, hvis meddelelserne sendes via en tredjepartstjeneste. Du kan bruge et WHOIS-opslagsværktøj til at finde ejeren af den blokerede IP-adresse.
