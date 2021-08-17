---
title: Undersøg alle brugernes aktiviteter
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: d05c8f02efc3bb92865880ea4a2338abaf7d70254f0b4bbfb566423e62b391dd
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/11/2021
ms.locfileid: "57898790"
---
# <a name="investigate-all-the-users-activities"></a>Undersøg alle brugernes aktiviteter

Sådan gør du:

1. Gør en af følgende handlinger:
   - I Microsoft 365 Overholdelsescenter på <https://compliance.microsoft.com> skal du gå til **Løsningsrevision** \> . Du kan også gå direkte til siden **Overvågning ved** hjælp af <https://compliance.microsoft.com/auditlogsearch> .
   - I Microsoft 365 Defender på <https://security.microsoft.com> skal du gå til **Overvågning**. Du kan også gå direkte til siden **Overvågning ved** hjælp af <https://security.microsoft.com/auditlogsearch> .

    > [!NOTE]
    > Hvis du ser en meddelelse om, at du skal aktivere funktionen, kan du slå den til nu. Hvis funktionen ikke er slået til, kan søgeresultaterne ikke trække data fra tidligere datoer.

2. På fanen **Søg** på siden **Overvågning** skal du konfigurere følgende indstillinger:
   - **Dato- og tidsinterval:** Markér dato/klokkeslæt-området i **felterne Start** **og** Slut.
   - **Aktiviteter:** Hvis du er interesseret i en bestemt aktivitet, skal du vælge den på listen. Ellers returnerer standardværdien **Vis resultater for alle** aktiviteter alle aktiviteter.
   - **Brugere:** Acceptér den tomme standardværdi for at returnere resultater for alle brugere, eller angiv en eller flere brugere.

3. Når du er færdig, skal du klikke på **Søg**. Aktiviteterne vises på den nye **overvågningssøgningsside.** Du får vist **IP-adressen**, **bruger og** **aktivitetsnavn.**

4. Hvis du vil hente resultaterne, skal du **vælge** \> **Eksportér Hent alle resultater**.

5. Vælg en aktivitet i resultaterne for at åbne pop op-dialogboksen med detaljer.

Du kan få mere at vide [under Søg i overvågningsloggen for at undersøge almindelige supportproblemer.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
