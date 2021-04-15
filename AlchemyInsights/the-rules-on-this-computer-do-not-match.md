---
title: 'Fejl: Reglerne på denne computer stemmer ikke overens'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782946"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Fejl: Reglerne på denne computer stemmer ikke overens

Hvis du vil have vist opdateret status for dette kendte problem, [skal du se Reglerne på denne computer svarer ikke til reglerne i Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Outlook-teamet har implementeret en rettelse i build 12928.10000. Rettelsen er allerede i Insider Fast og går til Månedlig kanal sidst i juni 2020. Når du har den rettede build, får du muligvis prompten "Hvilke regler vil du beholde" en sidste gang. Vælg Server, når du bliver bedt om det, og gå derefter tilbage til Outlook og genaktiver alle regler, der blev deaktiveret.

Indtil rettelsen er tilgængelig, skal du bruge følgende løsning:

**Løsning:** I de seneste rapporter er problemet mest forekommet hos personer, der kun har oprettet klientregler i skrivebordsversionen af Outlook. Hvis du fortsat løber ind i problemet, kan du overveje at slette reglerne og derefter kun oprette og redigere regler i OWA (Outlook Web App), indtil problemet er løst.

Hvis du ikke kan slette reglerne manuelt, kan du køre en Outlook-kommando, når du starter Outlook, ved at køre Outlook.exe /cleanrules. Dette sletter både klient- og serverreglerne. Det sletter alle reglerne for alle konti i Outlook-profilen. Denne kommando er yderligere dokumenteret i artiklen om kommandolinjeparametre.

