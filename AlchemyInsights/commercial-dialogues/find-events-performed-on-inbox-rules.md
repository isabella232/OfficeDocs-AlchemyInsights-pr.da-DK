---
title: Finde hændelser, der udføres på indbakkeregler
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
ms.openlocfilehash: d6a4eadd897dfae3b65ccda6363edfe9cef1c810
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58313493"
---
# <a name="find-events-performed-on-inbox-rules"></a>Finde hændelser, der udføres på indbakkeregler

Når indbakkeregler oprettes, ændres eller slettes, registreres hændelserne i overvågningsloggen. Sådan gennemser du dem:

1. Gør en af følgende handlinger:
   - I Microsoft 365 Overholdelsescenter på <https://compliance.microsoft.com> skal du gå til  \> **Løsningsrevision**. Du kan også gå direkte til siden **Overvågning ved** hjælp af <https://compliance.microsoft.com/auditlogsearch> .
   - I Microsoft 365 Defender på <https://security.microsoft.com> skal du gå til **Overvågning**. Du kan også gå direkte til siden **Overvågning ved** hjælp af <https://security.microsoft.com/auditlogsearch> .

    **Bemærk!** Hvis du ser en meddelelse om, at du skal aktivere overvågning, kan du slå det til nu. Hvis denne funktion ikke er slået til, kan søgeresultaterne ikke trække data fra tidligere datoer.
1. Vælg feltet Aktiviteter, og find Exchange postkasseaktiviteter, og vælg derefter New-InboxRule Opret indbakkeregel Outlook Web App. Når du er færdig, skal du klikke uden for ruden for at minimere ruden Aktiviteter.
1. Angiv datointervallet, og vælg derefter brugernavnet for den bruger, du vil undersøge, i feltet Brugere. Du kan vælge mere end én bruger ad gangen.
1. Vælg Søg. Aktiviteterne vises under Resultater.
1. Hvis du vil have vist detaljer, skal du vælge en aktivitet og derefter vælge Flere oplysninger. Under sektionen Parametre kan du se navnet på reglen, de indstillede betingelser og de handlinger, som reglen skal udføre.

2. På fanen **Søg** på siden **Overvågning** skal du konfigurere følgende indstillinger:
   - **Dato- og tidsinterval:** Markér dato/klokkeslæt-området i **felterne Start** **og** Slut.
   - **Aktiviteter:** Vælg **Ny indbakkeRegel om Opret indbakkeregel fra Outlook Web App**

3. Når du er færdig, skal du klikke på **Søg**. Aktiviteterne vises på den nye **overvågningssøgningsside.**

4. Vælg en aktivitet i resultaterne for at åbne pop op-dialogboksen med detaljer. Under sektionen **Parametre** kan du se navnet på reglen, de indstillede betingelser og de handlinger, som reglen skal udføre.

Du kan få mere at vide [under Søg i overvågningsloggen for at undersøge almindelige supportproblemer.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
