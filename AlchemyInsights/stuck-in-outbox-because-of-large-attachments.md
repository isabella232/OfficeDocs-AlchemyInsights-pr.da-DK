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
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441300"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Ret meddelelser, der sidder fast i udbakken

Vi anbefaler, at du starter med at køre scenariet ["Jeg har problemer med at sende, modtage eller finde mails"](https://aka.ms/SaRA-OutlookSendReceive) fra værktøjet [Microsoft support og genoprettelsesassistent](https://diagnostics.office.com/#/) .

Når en meddelelse sidder fast i udbakken, er de mest sandsynlige årsager:
- Store vedhæftede filer.
- Indstillingen **Send med det samme, når** den er tilsluttet er ikke aktiveret.

Sådan fjerner du store vedhæftede filer: 

1. I Outlook skal du vælge **Send/modtag** > **arbejde offline**. 
2. Vælg **Udbakke**i navigationsruden. Herfra kan du: 
    - Slet beskeden (Vælg den, og vælg derefter **Slet**).
    - Træk beskeden til mappen Kladder, dobbeltklik for at åbne den, og fjern den vedhæftede fil Vælg den, og vælg derefter **Slet**).
3. Hvis du får vist en fejlmeddelelse om, at Outlook forsøger at overføre meddelelsen, skal du lukke Outlook. Det kan tage et øjeblik at afslutte. Hvis Outlook ikke lukkes, skal du trykke på Ctrl + Alt + Delete og vælge **Start Jobliste**. Vælg fanen **processer** i Jobliste, Rul ned til Outlook. exe, og vælg **Afslut proces**.
4. Når Outlook er lukket, skal du genstarte det og gentage trin 2 og 3. 
5. Når du har fjernet den vedhæftede fil, skal du klikke på **Send/modtag** > **arbejde offline** for at genoptage arbejdet online. 

Meddelelser går også i stå i udbakken, når du klikker på **Send**, men du har ikke forbindelse. Klik på **Send/modtag** , og se på knappen **Arbejd offline** . Hvis det er blåt, er du afbrudt. Vælg den for at oprette forbindelse (knappen bliver hvid), og klik på **Send alle**.
 
Sådan aktiverer du **Send med det samme, når forbindelsen er oprettet**:
 
- Vælg **filindstillinger** > **** >  **Avanceret**.
I sektionen **Send og modtag** skal du vælge **Send med det samme, når du er tilsluttet**, og derefter vælge **OK**.
 
For udførlige oplysninger se:
- [Video: sende eller slette en fast e-mail](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [Mail forbliver i mappen Udbakke, indtil du manuelt starter en Send/modtag-handling i Outlook](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
