---
title: 'Fejl: Reglerne på denne computer stemmer ikke overens'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c0982da82826d1644f437b19e0d343a59d7ac473
ms.sourcegitcommit: e09af4285c6b81ca0a5320fdb811713ac25748c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/09/2020
ms.locfileid: "44664240"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Fejl: Reglerne på denne computer stemmer ikke overens

Hvis du vil se den opdaterede status for dette kendte problem, skal du se [Reglerne på denne computer stemmer ikke overens med reglerne på Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Outlook Team har implementeret en rettelse i Build 12928.10000. Rettelsen er allerede på Insider Fast og vil gå til Månedlig Channel i slutningen af juni 2020. Når du har den faste bygge du kan få prompten "Hvilke regler vil du beholde" en sidste gang. Vælg Server, når du bliver bedt om det, og gå derefter tilbage i Outlook, og genaktiver eventuelle regler, der er deaktiveret.

Indtil rettelsen er tilgængelig, skal du bruge følgende løsning:

**Løsning**: I de seneste rapporter er der opstået et problem for dem, der kun har oprettet klientregler i Outlook på computeren. Hvis du fortsætter med at løbe ind i problemet, kan du overveje at slette reglerne og derefter kun oprette og redigere regler i OWA (Outlook Web App), indtil problemet er løst.

Hvis du ikke kan slette reglerne manuelt, kan du køre en Outlook-kommando, når du starter Outlook, ved at køre Outlook.exe /cleanrules. Dette sletter både klient- og serverreglerne. Det vil slette alle reglerne for alle konti i Outlook-profilen. Denne kommando er yderligere dokumenteret i artiklen kommandolinjeparametre.

