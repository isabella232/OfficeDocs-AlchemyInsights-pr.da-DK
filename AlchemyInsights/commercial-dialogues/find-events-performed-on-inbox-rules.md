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
ms.openlocfilehash: 14a5a18bc1422572db567c9533fefe5a7e0120afd64df4a64623038cc063ce93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058644"
---
# <a name="find-events-performed-on-inbox-rules"></a>Finde hændelser, der udføres på indbakkeregler

Når indbakkeregler oprettes, ændres eller slettes, registreres hændelserne i overvågningsloggen. Sådan gennemgår du dem:

1. Gå til [Office 365 Security & Compliance Center.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Vælg Søg > søgning i overvågningsloggen.

    > [!NOTE]
    > Hvis du ser en meddelelse om, at du skal aktivere overvågning, skal du bare aktivere det nu. Hvis denne funktion ikke er aktiveret, kan søgeresultaterne ikke trække data fra tidligere datoer.
1. Vælg feltet Aktiviteter, find Exchange postkasseaktiviteter, og vælg derefter New-InboxRule Opret indbakkeregel Outlook Web App. Når du er færdig, skal du klikke uden for ruden for at minimere ruden Aktiviteter.
1. Angiv datointervallet, og vælg derefter brugernavnet for den bruger, du vil undersøge, i feltet Brugere. Du kan vælge mere end én bruger ad gangen.
1. Vælg Søg. Aktiviteterne vises under Resultater.
1. Hvis du vil have vist detaljer, skal du vælge en aktivitet og derefter vælge Flere oplysninger. Under sektionen Parametre kan du se navnet på reglen, de indstillede betingelser og de handlinger, som reglen skal udføre.

Du kan få mere at vide under Søg i Office 365 for at foretage fejlfinding af almindelige scenarier.