---
title: Fejl under afsendelse af e-mail, der er blokeret af SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: a16c998d2f289ea2da52454819f6677c405381a1
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/24/2019
ms.locfileid: "29463903"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Fejl under afsendelse af e-mail: klient-vært, der er blokeret ved hjælp af Spamhaus

Den IP-adresse, sendes meddelelsen er på en liste over blokerede websteder ejes af [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Årsager til at blive blokeret af Spamhaus omfatter skadet konti skadet maskiner dele en offentlig IP-adresse og politikker for internetudbyder (ISP). Mulige løsninger er:
  
- Blokerede indgående meddelelser til Office 365, hvor du styrer e-mail-kildeserveren, skal du finde årsagen og fjerne blokeringen fra webstedet Spamhaus.
    
- Blokerede indgående meddelelser til Office 365, hvor kilde-IP-adresse hører til en anden, skal ejeren af adressen blokeringen fjernes fra webstedet Spamhaus. Hvis IP-adressen på politikken Block liste (PBL), kan ejeren tildele en anden statisk IP-adresse eller fjerne adressen fra PBL.
    
- For blokerede udgående meddelelser fra dit domæne til Office 365, kan du modtager denne fejlmeddelelse, hvis meddelelser dirigeres gennem en 3. part service. Du kan bruge et værktøj til opslag af WHO-IS til at finde ejeren af blokerede IP-adresse.
    

