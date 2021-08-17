---
title: 1332 OWA – Indbakkeregel(er) udføres ikke for en postkasse
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: b05ed9f0ee8c18b49b5338c53e67a79f1bf65464385dfa0ebd0639172a1b18f2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040896"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>En indbakkeregel virker ikke som forventet

Bekræft følgende indstillinger i Outlook på internettet:

- En meddelelse kan kun omdirigeres, videresendes eller besvares automatisk baseret på indbakkeregler én gang. En omdirigeringsregel (en indbakkeregel eller regel for mailflow, også kaldet en transportregel) kan føje maksimalt ti modtagere af videresendelse til en meddelelse. Du kan få mere at vide [under Begrænsninger for journal-, transport- og indbakkeregler.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)

- Indbakkeregler fungerer ikke på den alternative journalpostkasse. Du kan finde flere oplysninger om den alternative journalpostkasse i [Alternativ journalboks](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Du kan løse disse problemer under [KB 2829319.](https://support.microsoft.com/kb/2829319)

Hvis de forrige problemer ikke gælder, skal du køre den diagnostiske Rapport over indbakkeregler, inden du eskalerer problemet til Microsoft Support:

1. Åbn postkassen i Outlook på internettet, og klik på <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Indstillinger**  >  **Vis alle Outlook Indstillinger**  >  **Mail**  >  **Regler**.

2. Nederst på siden skal du klikke på Hvis dine regler ikke **virker, skal du klikke her for at oprette en diagnosticeringsrapport.**
