---
title: Fjernelse af data og aftørring af enheder fra Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: f3614a41c1bc92184d7f8a11bd224310fef6aa0cabc8e1db1288bde01ca1cb5a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53922204"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Fjernelse af data og aftørring af enheder fra Intune

Fjernhandlingerne Enhedsopsletning og Sletning af enhed kan bruges til at fjerne virksomhedsdata, der administreres af Intune, eller til at udføre en nulstilling til fabriksindstilling og returnere enheden til standardindstillingerne.

1. Log på Microsoft 365 enhedshåndtering, og gå til **Enheder**  >  **alle enheder**.
2. Vælg den enhed, du vil slette.
3. Vælg den type fjernsletning, du vil udføre. Tilbagetrækning sletter kun virksomhedsoplysninger, mens komplette sletninger gendanner enheden til fabriksindstillingerne.
4. Vælg **Ja for** at bekræfte. Indtil sletningen afsluttes, vises enhedsstatussen Tilbagetrækning *afventer*.
    Når handlingen er fuldført, vises mobilenheden ikke længere på listen over administrerede enheder.

> [!NOTE]
> Firmadata kan ikke fjernes fra enheder, der ER FORBUNDET til Azure AD. 

Du kan finde detaljerede oplysninger om effekten af handlingerne Tilbagetrækning og Sletning, herunder hvad der bevares, og hvad der slettes, i følgende dokumentation:

- [Fjern enheder ved at slette, trække dem tilbage eller manuelt ophæve tilmeldingen af enheden.](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe)
- [Sådan slettes kun virksomhedsdata fra Intune-administrerede apps](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [Slet alle data fra en macOS-enhed](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).