---
title: 1332 OWA - Indbakke-regler ikke udføres for en postkasse
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: f090d0a9d84bc6a4d1a1f4c0af55102d4b0ddfbe
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/15/2019
ms.locfileid: "28283213"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>En regel for indbakke virker ikke som forventet

Kontroller følgende indstillinger:
  
- En meddelelse kan omdirigeres, videresendte eller besvarede automatisk baseret på indbakkereglerne kun én gang. En omdirigere regel (en regel for Indbakke eller flow postregel, også kendt som hovedregel transport) kan tilføje op til ti modtagere i videresende en meddelelse. Yderligere oplysninger finder du under [grænser for kladden, Transport, og Indbakke](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).
    
- Indbakkeregler fungerer ikke på den alternative journalføring postkasse. Yderligere oplysninger om alternative journalføring postkassen, se [alternativ journalføring postkasse](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).
    
Du kan løse disse problemer ved at se [KB 2829319](https://support.microsoft.com/kb/2829319).
  
Hvis du ikke anvender de tidligere problemer, køre Indbakke regel Diagnosticeringsrapport, før du eskalere problemet til Microsoft Support:
  
1. Åbne postkassen i Outlook på internettet, og klik på **Indstillinger for** \> **Indstillinger** \> **Organiser e-mail** \> **af regler for indbakken**.
    
2. Klik på **Hvis reglerne ikke arbejder Klik her for at generere en diagnosticeringsrapport**nederst på siden.
    

