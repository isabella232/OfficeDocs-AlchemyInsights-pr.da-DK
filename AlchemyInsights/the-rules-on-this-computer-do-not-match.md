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
ms.openlocfilehash: b77573e9d94195e1f0ef4a1566c45a30d53b7e68e502aeb834e2ca5b9e6c5c76
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981107"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Fejl: Reglerne på denne computer stemmer ikke overens

Hvis du vil have vist opdateret status for dette kendte problem, skal du [se Reglerne på denne computer svarer ikke til reglerne på Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Teamet Outlook en rettelse i build 12928.10000. Rettelsen er allerede i Insider Fast og går til Månedlig kanal sidst i juni 2020. Når du har den rettede build, får du muligvis prompten "Hvilke regler vil du beholde" en sidste gang. Vælg Server, når du bliver bedt om det, og gå derefter tilbage Outlook og genaktiver alle regler, der er blevet deaktiveret.

Indtil rettelsen er tilgængelig, skal du bruge følgende løsning:

**Løsning:** I de seneste rapporter er problemet mest forekommet hos personer, der kun har oprettet klientregler Outlook computeren. Hvis du fortsat løber ind i problemet, kan du overveje at slette reglerne og derefter kun oprette og redigere regler i OWA (Outlook Web App), indtil problemet er løst.

Hvis du ikke kan slette reglerne manuelt, kan du køre en Outlook, når du starter Outlook ved at køre Outlook.exe /cleanrules. Dette sletter både klient- og serverreglerne. Det sletter alle reglerne for alle konti i Outlook Profil. Denne kommando er yderligere dokumenteret i artiklen om kommandolinjeparametre.

