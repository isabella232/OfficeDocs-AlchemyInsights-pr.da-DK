---
title: Har du brug for hjælp til grænser for afsendelse af e-mails?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 7f563df313c869d18c3e4240d271c649a74914af
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357398"
---
# <a name="need-help-with-email-sending-limits"></a>Har du brug for hjælp til grænser for afsendelse af e-mails?

Nedenfor er **by-design afsendelse grænser håndhæves** i tjenesten. Du kan finde flere oplysninger om disse grænser [her](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).

- For at modvirke levering af uopfordrede massemeddelelser anvender vi hastighedsgrænser pr. bruger **på alle udgående og interne meddelelser**. På tværs af alle lagervarer er denne grænse **10.000 modtagere om dagen.**  Kunder, der har brug for at sende en legitim massekommerciel e-mail (f.eks. kundenyhedsbreve), skal bruge tredjepartsudbydere, der specialiserer sig i disse tjenester.
    - **Bemærk:** Når grænsen for modtagerhastighed er nået, kan meddelelser ikke sendes fra postkassen, før antallet af modtagere, der er sendt meddelelser inden for de seneste 24 timer, falder til under grænsen. Brugeren kan ikke sende meddelelser før dette tidspunkt.
- Grænsen for meddelelseshastighed på **30 meddelelser pr. minut** anvendes på tværs af alle lagervarer. Dette bestemmer, hvor mange meddelelser en bruger kan sende fra sin Exchange Online-konto inden for en bestemt periode.
- Det maksimale antal modtagere, der er tilladt i felterne **Til, Cc og Bcc** for en enkelt mail på tværs af alle Lagervarer, er **1000 modtagere**. Hvis du vil tilpasse denne grænse, skal du gå [hertil](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).
