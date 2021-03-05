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
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481721"
---
# <a name="find-the-ip-address-in-audit-log"></a>Find IP-adressen i overvågningsloggen

1. Den IP-adresse, der svarer til en aktivitet, der er udført af en bruger eller administrator, vises i overvågningsloggen. Klientoplysningerne logføres også. Sådan identificerer du IP-adressen:

1. Gå til [Office 365 Security & Compliance Center.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Vælg **søgning i**  >  **[overvågningsloggen.](https://go.microsoft.com/fwlink/?linkid=2103759)**
    > [!NOTE]
    > Hvis du ser en meddelelse om, at du skal aktivere overvågning, kan du aktivere det nu. Hvis denne funktion ikke er aktiveret, vil søgeresultaterne ikke kunne trække data fra tidligere datoer.
1. Hvis du er interesseret i en bestemt aktivitet, skal du vælge den på **listen** Aktiviteter. Ellers returneres alle aktiviteter som standard for den valgte bruger. Bemærk, at visse aktiviteter muligvis ikke kan vælges i **menuen** Aktiviteter. disse overvågningselementer returneres dog, hvis **Vis resultater for alle aktiviteter** er valgt (standardindstilling).
1. Angiv datointervallet, og vælg **brugernavnet for** den bruger, du vil undersøge, i feltet Brugere.
1. Vælg **Søg.** Aktiviteterne vises under **Resultater.** Du kan se IP-adressen for hver aktivitet.
1. Hvis du vil have vist detaljer, skal du vælge en aktivitet og derefter **vælge Flere oplysninger.**

Hvis du vil have mere at vide, skal du [se Søge i Office 365-overvågningsloggen for at foretage fejlfinding af almindelige scenarier.](https://go.microsoft.com/fwlink/?linkid=2103944)