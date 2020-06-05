---
title: 1332 OWA - Indbakkeregel(er) udføres ikke for en postkasse
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 9abdcdcb33d39b8b9fe2df80f0c15a8b55e465fd
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/05/2020
ms.locfileid: "44576554"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>En indbakkeregel fungerer ikke som forventet

Kontroller følgende indstillinger i Outlook på internettet:

- En meddelelse kan kun omdirigeres, videresendes eller besvares automatisk baseret på indbakkeregler én gang. En omdirigeringsregel (en indbakkeregel eller mailflowregel, også kaldet en transportregel) kan maksimalt føje ti videresendelsesmodtagere til en meddelelse. Yderligere oplysninger finder du i [Regelgrænser for journal, transport og indbakke](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Indbakkeregler fungerer ikke på den alternative journalpostkasse. Yderligere oplysninger om den alternative journalpostkasse finder du i [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Du kan løse disse problemer ved at se [KB 2829319](https://support.microsoft.com/kb/2829319).

Hvis de tidligere problemer ikke gælder, skal du køre rapporten til diagnosticering af indbakkeregel, før du eskalerer problemet til Microsoft Support:

1. Åbne postkassen i Outlook på internettet, og klik på <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Indstillinger**  >  **Få vist alle Outlook-indstillinger**  >  **Dagens e-avis**  >  **Regler**.

2. Nederst på siden skal du klikke på **Hvis reglerne ikke fungerer, skal du klikke her for at generere en diagnosticeringsrapport**.
