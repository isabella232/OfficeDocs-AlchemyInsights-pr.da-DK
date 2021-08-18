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
ms.openlocfilehash: 92673c4a2a0e0faa98d3ade5ca1f6aa687d4c94a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331035"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Fjernelse af data og aftørring af enheder fra Intune

Fjernhandlingerne Enhedssletning og Sletning af enhed kan bruges til at fjerne virksomhedsdata, der administreres af Intune, eller til at udføre en nulstilling til fabriksindstilling og returnere enheden til standardindstillingerne.

1. Log på Microsoft 365 administration af enheder, og gå til **Enheder**  >  **alle enheder**.
2. Vælg den enhed, du vil slette.
3. Vælg den type fjernsletning, du vil udføre. Tilbagetrækning sletter kun virksomhedsoplysninger, mens komplette sletninger gendanner enheden til fabriksindstillingerne.
4. Vælg **Ja for** at bekræfte. Indtil sletningen afsluttes, vises enhedsstatussen Tilbagetrækning *afventer*.
    Når handlingen er fuldført, vises mobilenheden ikke længere på listen over administrerede enheder.

**Bemærk!** Firmadata kan ikke fjernes fra enheder, DER ER FORBUNDET til Azure AD. 

Du kan finde detaljerede oplysninger om effekten af handlingerne Tilbagetrækning og Sletning, herunder hvad der bevares, og hvad der slettes, i følgende dokumentation:

- [Fjern enheder ved at slette, trække dem tilbage eller manuelt ophæve tilmeldingen af enheden.](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe)
- [Sådan slettes kun virksomhedsdata fra Intune-administrerede apps](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [Slet alle data fra en macOS-enhed](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).