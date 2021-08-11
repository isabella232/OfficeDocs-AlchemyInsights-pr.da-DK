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
ms.openlocfilehash: 8d656d5660b7c6e6d32d32a06c3dbf49c45e4ca04c4422128f1c4ea62413afa1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53967327"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>Læs overvågningslogfilerne for slettede hændelser

Sådan gør du:

1. Gå til [Office 365 Security & Compliance Center.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Vælg **Søgning i**  >  [**overvågningslogsøgning**](https://go.microsoft.com/fwlink/?linkid=2103759).
    > [!NOTE]
    > Hvis du ser en meddelelse om, at du skal aktivere funktionen, kan du slå den til nu. Hvis funktionen ikke er slået til, kan søgeresultaterne ikke trække data fra tidligere datoer.
1. Vælg **Aktiviteter**, og find derefter **Exchange postkasseaktiviteter**. Vælg indstillingerne **Slettet post fra mappen Slettet** post og Flyttede meddelelser til mappen **Slettet** post. Når du er færdig, skal du klikke uden for ruden for at minimere **ruden** Aktiviteter.
1. Angiv datointervallet, og markér **brugernavnet** for den bruger, du vil undersøge, i feltet Brugere. Du kan vælge mere end én bruger ad gangen.
1. Vælg **Søg**. Aktiviteterne vises under **Resultater.**
1. Hvis du vil se detaljerne, skal du vælge en aktivitet og derefter **vælge Flere oplysninger**. Yderligere oplysninger om det slettede element, f.eks. emnelinjen og placeringen af elementet,  da det blev slettet, vises i feltet BerørteWebsteder.
    > [!NOTE]
    > Du kan ikke gendanne slettede elementer ved hjælp af overvågningslogfunktionen. Hvis du vil gendanne slettede elementer, [skal du se Gendan slettede elementer eller mails i Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).

Du kan få mere at vide [under Søg i Office 365 for at foretage fejlfinding af almindelige scenarier.](https://go.microsoft.com/fwlink/?linkid=2103944)
