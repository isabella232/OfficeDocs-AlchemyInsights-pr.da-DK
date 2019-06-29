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
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Fejl under afsendelse af e-mail: klient-vært, der er blokeret ved hjælp af Spamhaus

Den IP-adresse, sendes meddelelsen er på en liste over blokerede websteder ejes af [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Årsager til at blive blokeret af Spamhaus omfatter skadet konti skadet maskiner dele en offentlig IP-adresse og politikker for internetudbyder (ISP). Mulige løsninger er:
  
- Blokerede indgående meddelelser til Office 365, hvor du styrer e-mail-kildeserveren, skal du finde årsagen og fjerne blokeringen fra webstedet Spamhaus.

- Blokerede indgående meddelelser til Office 365, hvor kilde-IP-adresse hører til en anden, skal ejeren af adressen blokeringen fjernes fra webstedet Spamhaus. Hvis IP-adressen på politikken Block liste (PBL), kan ejeren tildele en anden statisk IP-adresse eller fjerne adressen fra PBL.

- For blokerede udgående meddelelser fra dit domæne til Office 365, kan du modtager denne fejlmeddelelse, hvis meddelelser dirigeres gennem en 3. part service. Du kan bruge et værktøj til opslag af WHO-IS til at finde ejeren af blokerede IP-adresse.
