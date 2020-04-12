---
title: Sidder fast i udbakken på grund af store vedhæftede filer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
- "9002385"
- "4645"
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232624"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Rette meddelelser, der sidder fast i udbakken

Vi anbefaler, at du starter med at køre scenariet ["Jeg har problemer med at sende, modtage eller finde mails"](https://aka.ms/SaRA-OutlookSendReceive) fra [værktøjet Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) på den berørte computer.

Når en meddelelse sidder fast i udbakken, er den mest sandsynlige årsag en stor vedhæftet fil, eller indstillingen "Send med det samme, når den er tilsluttet" er ikke aktiveret.

**Fjerne den store vedhæftede fil**

1. Klik på **Send/modtag** > **arbejde offline**. 
2. Klik på **Udbakke**i navigationsruden . Herfra kan du: 
    - Slet meddelelsen. Du skal blot markere den og klikke på **Slet**.
    - Træk meddelelsen til **kladdemappen**, dobbeltklik for at åbne meddelelsen, og slet den vedhæftede fil (klik på den, og klik på **Slet**).
3. Hvis en fejl fortæller dig, at Outlook forsøger at sende meddelelsen, skal du lukke Outlook. Det kan tage et øjeblik at afslutte. Hvis Outlook ikke lukker, skal du trykke **på Ctrl+Alt+Delete** og klikke på **Start Jobliste**. Vælg fanen **Processer** i Jobliste, rul ned til outlook.exe, og klik på **Afslut proces**.
4. Når Outlook er lukket, skal du genstarte Outlook og gentage trin 2-3. 
5. Når du har fjernet den vedhæftede fil, skal du klikke på **Send/modtag** > **arbejde offline** for at fravælge knappen og for at fortsætte med at arbejde online. 

Meddelelser sidder også fast i udbakken, når du klikker på **Send**, men du har ikke forbindelse. Klik på **Send/modtag,** og se på knappen **Arbejd offline.** Hvis den er blå, er forbindelsen afbrudt. Klik på den for at oprette forbindelse (knappen bliver hvid), og klik på **Send alle**.
 
**Aktiver Send med det samme, når der er oprettet forbindelse**
 
1. Klik på **Indstillinger**under fanen Filer .

2. Klik på **Avanceret**i dialogboksen Outlook-indstillinger .

3. Klik på i sektionen Send og modtag for at aktivere **Send med det samme, når der er oprettet forbindelse**. Klik på **OK**.
 
Du kan finde flere oplysninger under:
- [Video: Sende eller slette en fast låst mail](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [Mail forbliver i mappen Udbakke, indtil du manuelt starter en send/modtag-handling i Outlook](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
