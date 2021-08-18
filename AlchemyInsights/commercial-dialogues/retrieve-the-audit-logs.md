---
title: Hent overvågningslogfilerne
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 88d28898923c1381c001c15445da90901b7e8761
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320437"
---
# <a name="retrieve-the-audit-logs"></a>Hent overvågningslogfilerne

Når du åbner overvågningsloggen første gang, vil den være tom. Du skal udføre en søgning for at se, hvad der er der. Sådan kan du udføre en generel søgning efter alle aktiviteter:

1. Gør en af følgende handlinger:
   - I Microsoft 365 Overholdelsescenter på <https://compliance.microsoft.com> skal du gå til  \> **Løsningsrevision**. Du kan også gå direkte til siden **Overvågning ved** hjælp af <https://compliance.microsoft.com/auditlogsearch> .
   - I Microsoft 365 Defender på <https://security.microsoft.com> skal du gå til **Overvågning**. Du kan også gå direkte til siden **Overvågning ved** hjælp af <https://security.microsoft.com/auditlogsearch> .

2. På fanen **Søg** på siden **Overvågning** skal du konfigurere følgende indstillinger:
   - **Dato- og tidsinterval:** Markér dato/klokkeslæt-området i **felterne Start** **og** Slut.
   - **Aktiviteter:** **Bekræft, at Vis resultater for alle aktiviteter** er markeret.
   - **Brugere:** Acceptér den tomme standardværdi for at returnere resultater for alle brugere, eller angiv en eller flere brugere.

3. Når du er færdig, skal du klikke på **Søg**. Aktiviteterne vises på den nye **overvågningssøgningsside.**

4. Vælg en aktivitet i resultaterne for at åbne pop op-dialogboksen med detaljer. Du kan se flere oplysninger, f.eks Klient, Bruger, der udførte handlingen osv.

Du kan få mere at vide [under Søg i overvågningsloggen for at undersøge almindelige supportproblemer.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
