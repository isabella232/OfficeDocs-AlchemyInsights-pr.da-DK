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
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Fejl ved afsendelse af mail: klient vært blokeret ved hjælp af spam Haus

Den IP-adresse, der sendte meddelelsen, er på en blokliste, der ejes af [spam Haus](https://go.microsoft.com/fwlink/p/?linkid=123245). Grunde til at blive blokeret af spam Haus omfatter skadede konti, kompromitterede maskiner, der deler en offentlig IP-adresse og en internetudbyder (ISP)-politikker. Mulige rettelser:
  
- For blokerede indgående meddelelser, hvor du styrer kilde mailserveren, skal du finde årsagen og fjerne blokken fra spam Haus websted.

- For blokerede indgående meddelelser, hvor kildens IP-adresse tilhører en anden, skal adresse ejeren fjerne blokken fra spam Haus websted. Hvis IP-adressen er på listen politik blok (PBL), kan ejeren tildele en anden statisk IP-adresse eller fjerne adressen fra PBL.

- For blokerede udgående meddelelser fra dit domæne, der er knyttet til Microsoft, kan du få denne fejl, hvis meddelelserne sendes via en tredjepartstjeneste. Du kan bruge et WHOIS-opslagsværktøj til at finde den blokerede IP-adresse ejer.
