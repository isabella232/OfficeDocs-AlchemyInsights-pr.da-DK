---
title: Find IP-adressen i overvågningsloggen
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
ms.openlocfilehash: 5b58803719df700290f495cb2d2d6742f072420a2a1d393534ca165bb5a14fbb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54017126"
---
# <a name="find-the-ip-address-in-audit-log"></a>Find IP-adressen i overvågningsloggen

1. Den IP-adresse, der svarer til en aktivitet, der er udført af en bruger eller administrator, vises i overvågningslogfilerne. Klientoplysningerne logføres også. Sådan identificerer du IP-adressen:

1. Gå til [Office 365 Security & Compliance Center.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Vælg **Søgning i**  >  **[overvågningslogsøgning](https://go.microsoft.com/fwlink/?linkid=2103759)**.
    > [!NOTE]
    > Hvis du ser en meddelelse om, at du skal aktivere overvågning, skal du bare aktivere det nu. Hvis denne funktion ikke er aktiveret, vil søgeresultaterne ikke kunne trække data fra tidligere datoer.
1. Hvis du er interesseret i en bestemt aktivitet, skal du vælge den på **listen** Aktiviteter. Ellers returneres alle aktiviteter som standard for den valgte bruger. Bemærk, at visse aktiviteter muligvis ikke kan vælges fra **menuen** Aktiviteter. disse overvågningselementer returneres dog, hvis **Vis resultater for alle aktiviteter** er valgt (standardindstilling).
1. Angiv datointervallet, og vælg **brugernavnet** for den bruger, du vil undersøge, i feltet Brugere.
1. Vælg **Søg**. Aktiviteterne vises under **Resultater.** Du kan se IP-adressen for hver aktivitet.
1. Hvis du vil have vist detaljer, skal du vælge en aktivitet og derefter **vælge Flere oplysninger**.

Få mere at vide under Søg i Office 365 [for at foretage fejlfinding af almindelige scenarier.](https://go.microsoft.com/fwlink/?linkid=2103944)