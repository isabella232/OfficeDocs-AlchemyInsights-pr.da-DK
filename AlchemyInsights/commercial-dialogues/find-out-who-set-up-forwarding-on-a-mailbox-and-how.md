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
ms.openlocfilehash: 6243e787bb6b51f26cf22782d9ec80f946430b864f53de7ea626b7166a674d2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988173"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Find ud af, hvem der har konfigureret videresendelse på en postkasse, og hvordan

Hvis ekstern videresendelse blev angivet på en postkasse, overvåges aktiviteten som en del Set-Mailbox cmdlet'en. Sådan finder du aktiviteten i overvågningsloggen:

1. Gå til [Office 365 Security & Compliance Center.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Vælg **Søgning i** >  **overvågningslogsøgning**.
    > [!NOTE]
    > Hvis du ser en meddelelse om, at du skal aktivere overvågning, skal du bare aktivere det nu. Hvis denne funktion ikke er aktiveret, kan søgeresultaterne ikke trække data fra tidligere datoer.
1. Sørg for, **at feltet** Aktiviteter er indstillet **til Vis resultater for alle** aktiviteter (standard). Angiv datointervallet. Du behøver ikke at angive et brugernavn.
1. Vælg **Søg**. Aktiviteterne vises under **Resultater.**
1. Vælg **Filtrer** resultater , og angiv **derefter Set-mailbox** i **filterfeltet** Aktivitet. Dette returnerer alle **Set-Mailbox-aktiviteter.**
1. Hvis du vil se detaljerne, skal du vælge en aktivitet og derefter **vælge Flere oplysninger**. Under **Parametre** kan du se den mailadresse til videresendelse, der blev angivet på postkassen. UserID **repræsenterer** den bruger, der har konfigureret ekstern videresendelse i postkassen.
Du kan få mere at vide [under Søg i Office 365 for at foretage fejlfinding af almindelige scenarier.](https://go.microsoft.com/fwlink/?linkid=2103944)