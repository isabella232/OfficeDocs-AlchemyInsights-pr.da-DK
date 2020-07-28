---
title: Fjernelse af data og aftørring af enheder fra Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439157"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Fjernelse af data og aftørring af enheder fra Intune

Fjernhandlingerne Device Retire og Device Wipe kan bruges til at fjerne firmadata, der administreres af Intune, eller til at udføre en fabriksnulstilling og returnere enheden til standardindstillingerne.

1. Log på Microsoft 365 Device Management, og gå til **Enheder**  >  **alle enheder**.
2. Vælg den enhed, du vil slette.
3. Vælg den type fjernsletning, du vil udføre. Udgå sletter kun organisatoriske oplysninger, mens fuld klude gendanne enheden til sine fabriksindstillinger.
4. Vælg **Ja for** at bekræfte. Indtil sletningen er færdig, vises statussen Enhedshandling som Afventer pension.</br>
    Når handlingen er fuldført, kan du ikke længere se mobilenheden på listen over administrerede enheder.

**Bemærk:** Virksomhedsdata kan ikke fjernes fra enheder, der er tilsluttet Azure AD.

Du kan finde alle oplysninger om effekten af handlingerne Gå på pension og slette, herunder hvad der bevares, og hvad der slettes, under Fjerne enheder [ved hjælp af sletning, udgå eller automatisk](https://docs.microsoft.com/intune/devices-wipe)fjernelse af enheden .

Hvis du vil slette alle data fra en macOS-enhed, skal [du se Slette alle data fra en macOS-enhed](https://docs.microsoft.com/intune/device-erase).