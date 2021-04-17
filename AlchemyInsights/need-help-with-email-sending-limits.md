---
title: Har du brug for hjælp til grænser for afsendelse af mail?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: b5bdfbf818328c97ec93b3468aeedcbe88e03913
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836273"
---
# <a name="need-help-with-email-sending-limits"></a>Har du brug for hjælp til grænser for afsendelse af mail?

Nedenfor er de **designbaserede grænser for afsendelse** i tjenesten. Du kan finde flere oplysninger om disse begrænsninger [her.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits)

- For at afholde os fra at levere uopfordrede massemeddelelser, anvender vi satsbegrænsninger pr. bruger **på alle udgående og interne meddelelser.** På tværs af alle SKU'er er **denne grænse 10.000 modtagere pr. dag.**  Kunder, der har brug for at sende legitime kommercielle massemails (f.eks. kundebrevbrev), bør benytte tredjepartsudbydere, der er specialiserede i disse tjenester.
    - **Bemærk!** Når du når grænsen for modtagerhastigheden, kan meddelelser ikke sendes fra postkassen, før antallet af modtagere, der er blevet sendt meddelelser inden for de seneste 24 timer, falder under grænsen. Brugeren vil ikke kunne sende meddelelser før dette tidspunkt.
- Grænsen for **meddelelsessats på 30 meddelelser i minuttet** anvendes på tværs af alle SKU'er. Dette bestemmer, hvor mange meddelelser en bruger kan sende fra sin Exchange Online-konto inden for en bestemt periode.
- Det maksimale antal modtagere, der er tilladt i felterne **Til, Cc** og Bcc for en enkelt mail på tværs af alle SKU'er, er **1000 modtagere.** Hvis du vil tilpasse denne grænse, skal du [gå hertil.](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228)
