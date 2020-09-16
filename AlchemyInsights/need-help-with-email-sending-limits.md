---
title: Har du brug for hjælp til mail afsende begrænsninger?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 66ff82afd7b44ef5fd4943bfc794c2fa35bbfa9e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702357"
---
# <a name="need-help-with-email-sending-limits"></a>Har du brug for hjælp til mail afsende begrænsninger?

Herunder er de **begrænsninger, som** tildeles ved at håndhæves i tjenesten. Yderligere oplysninger om disse begrænsninger beskrives [her](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).

- For at forhindre levering af meddelelser, der ikke blev anmodet om, gælder det, at vi anvender **tilsvarende begrænsninger pr. bruger på alle udgående og interne meddelelser**. På tværs af alle lager numre er denne grænse **10.000 modtagere om dagen**.  Kunder, der har brug for at sende ægte kommercielle mails (f. eks. kunde-nyhedsbreve), skal anvende tredjepartsudbydere, der er specialiseret i disse tjenester.
    - **Bemærk**! når grænsen for modtager satsen er nået, kan meddelelser ikke sendes fra postkassen, før antallet af modtagere, der er blevet sendt meddelelser inden for de seneste 24 timer, falder ned under grænsen. Brugeren vil ikke kunne sende meddelelser før dette tidspunkt.
- Grænsen for meddelelses hastighed på **30 meddelelser pr. minut** anvendes på tværs af alle SKU'er. Dette bestemmer, hvor mange meddelelser en bruger kan sende fra sin Exchange Online-konto inden for en bestemt periode.
- Det **maksimale antal modtagere, der er tilladt i felterne til, CC og Bcc** for en enkelt mail, er **1000 modtagere**på tværs af alle SKU'er. Du kan tilpasse denne grænse ved at gå [hertil](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).
