---
title: Find ud af, hvem der har konfigureret videresendelse på en postkasse, og hvordan
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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429418"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Find ud af, hvem der har konfigureret videresendelse på en postkasse, og hvordan

Hvis ekstern videresendelse blev angivet på en postkasse, overvåges aktiviteten som en del Set-Mailbox cmdlet'en. Sådan finder du aktiviteten i overvågningsloggen:

1. Gå til [Office 365 Security & Compliance Center.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Vælg **søgning i** >  **overvågningsloggen.**
    > [!NOTE]
    > Hvis du ser en meddelelse om, at du skal aktivere overvågning, kan du aktivere det nu. Hvis denne funktion ikke er slået til, kan søgeresultaterne ikke trække data fra tidligere datoer.
1. Sørg for, **at feltet** Aktiviteter er indstillet **til At vise resultater for alle aktiviteter** (standarden). Angiv datointervallet. Du behøver ikke at angive et brugernavn.
1. Vælg **Søg.** Aktiviteterne vises under **Resultater.**
1. Vælg **Filtrer** resultater, og angiv **derefter Set-mailbox** i **feltet Aktivitetsfilter.** Dette returnerer alle **Set-Mailbox-aktiviteter.**
1. Hvis du vil have vist detaljerne, skal du vælge en aktivitet og derefter **vælge Flere oplysninger.** Under **Parametre** kan du se den mailadresse til videresendelse, der blev angivet på postkassen. **Bruger-id'et** repræsenterer den bruger, der har konfigureret ekstern videresendelse på postkassen.
Hvis du vil have mere at vide, [skal du se Søge i Office 365-overvågningsloggen for at foretage fejlfinding af almindelige scenarier.](https://go.microsoft.com/fwlink/?linkid=2103944)