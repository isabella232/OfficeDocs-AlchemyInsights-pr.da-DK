---
title: Find hændelser, der udføres på indbakkeregler
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
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481716"
---
# <a name="find-events-performed-on-inbox-rules"></a>Find hændelser, der udføres på indbakkeregler

Når indbakkeregler oprettes, ændres eller slettes, registreres hændelserne i overvågningsloggen. Sådan gennemgår du dem:

1. Gå til [Office 365 Security & Compliance Center.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Vælg Søg > søgning i overvågningsloggen.

    > [!NOTE]
    > Hvis du ser en meddelelse om, at du skal aktivere overvågning, kan du aktivere det nu. Hvis denne funktion ikke er slået til, kan søgeresultaterne ikke trække data fra tidligere datoer.
1. Vælg feltet Aktiviteter, find Exchange-postkasseaktiviteter, og vælg derefter New-InboxRule Opret indbakkeregel fra Outlook Web App. Når du er færdig, skal du klikke uden for ruden for at minimere ruden Aktiviteter.
1. Angiv datointervallet, og vælg derefter brugernavnet for den bruger, du vil undersøge, i feltet Brugere. Du kan vælge mere end én bruger ad gangen.
1. Vælg Søg. Aktiviteterne vises under Resultater.
1. Hvis du vil have vist detaljer, skal du vælge en aktivitet og derefter vælge Flere oplysninger. Under sektionen Parametre kan du se navnet på reglen, betingelser, der er angivet, og de handlinger, som reglen skal udføre.

Hvis du vil have mere at vide, skal du se Søge i Office 365-overvågningsloggen for at foretage fejlfinding af almindelige scenarier.