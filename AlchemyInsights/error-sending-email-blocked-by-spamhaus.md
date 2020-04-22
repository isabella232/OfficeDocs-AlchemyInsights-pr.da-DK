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
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Fejl under afsendelse af mail: Klientvært blokeret ved hjælp af Spamhaus

Den IP-adresse, der sendte meddelelsen, findes på en blokeringsliste, der ejes af [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Årsagerne til at blive blokeret af Spamhaus omfatter kompromitterede konti, kompromitterede maskiner, der deler en offentlig IP-adresse, og politikker for internetudbydere. Mulige rettelser er:
  
- For blokerede indgående meddelelser, hvor du styrer kildemailserveren, skal du finde årsagen og fjerne blokeringen fra Spamhaus's websted.

- For blokerede indgående meddelelser, hvor kildens IP-adresse tilhører en anden, skal adresseejeren fjerne blokeringen fra Spamhaus's websted. Hvis IP-adressen er på PBL (Policy Block List), kan ejeren tildele en anden statisk IP-adresse eller fjerne adressen fra PBL'en.

- For blokerede udgående meddelelser fra dit domæne, der er tilsluttet Microsoft, kan du få vist denne fejl, hvis meddelelserne dirigeres via en tredjepartstjeneste. Du kan bruge et WHOIS-opslagsværktøj til at finde den blokerede ip-adresseejer.
