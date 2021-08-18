---
title: Læs overvågningslogfilerne for slettede hændelser
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
ms.openlocfilehash: ec8f845f599e397814bc9077c3fe59edb5324192
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324727"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>Læs overvågningslogfilerne for slettede hændelser

Sådan gør du:

1. Gør en af følgende handlinger:
   - I Microsoft 365 Overholdelsescenter på <https://compliance.microsoft.com> skal du gå til  \> **Løsningsrevision**. Du kan også gå direkte til siden **Overvågning ved** hjælp af <https://compliance.microsoft.com/auditlogsearch> .
   - I portalen Microsoft 365 Defender på <https://security.microsoft.com> skal du gå til **Overvågning**. Du kan også gå direkte til siden **Overvågning ved** hjælp af <https://security.microsoft.com/auditlogsearch> .

    **Bemærk!** Hvis du ser en meddelelse om, at du skal aktivere funktionen, kan du slå den til nu. Hvis funktionen ikke er slået til, kan søgeresultaterne ikke trække data fra tidligere datoer.

2. På fanen **Søg** på siden **Overvågning** skal du konfigurere følgende indstillinger:
   - **Dato- og tidsinterval:** Markér dato/klokkeslæt-området i **felterne Start** **og** Slut.
   - **Aktiviteter:** **Exchange postkasseaktiviteter,** og vælg derefter følgende værdier:
     - **Slettede meddelelser fra mappen Slettet post**
     - **Meddelelser flyttet til mappen Slettet post**

       Når du er færdig, skal du klikke uden for ruden for at minimere **ruden** Aktiviteter.

   - **Brugere:** Acceptér den tomme standardværdi for at returnere resultater for alle brugere, eller angiv en eller flere brugere.

3. Når du er færdig, skal du klikke på **Søg**. Aktiviteterne vises på den nye **overvågningssøgningsside.**

4. Vælg en aktivitet i resultaterne for at åbne pop op-dialogboksen med detaljer. Yderligere oplysninger om det slettede element, f.eks. emnelinjen og placeringen af elementet,  da det blev slettet, vises i feltet BerørteWebsteder.

   **Bemærk!** Du kan ikke gendanne slettede elementer ved hjælp af overvågningslogfunktionen. Hvis du vil gendanne slettede elementer, [skal du se Gendan slettede mails i Outlook på internettet](https://support.microsoft.com/office/recover-deleted-email-messages-in-outlook-on-the-web-a8ca78ac-4721-4066-95dd-571842e9fb11).

Få mere at vide under [Søg i overvågningsloggen for at undersøge almindelige supportproblemer.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
