---
title: Fjern data og aftørring af enheder fra Intune
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
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416307"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Fjern data og aftørring af enheder fra Intune

Tilbagetrulning af enhed og fjernsletning af enhed kan bruges til at fjerne virksomhedsdata, der administreres af Intune, eller til at udføre en nulstilling til fabriksindstilling og returnere enheden til standardindstillingerne.

1. Log på Microsoft 365 Enhedshåndtering, og gå til **Enheder**  >  **på alle enheder.**
2. Vælg den enhed, du vil slette.
3. Vælg den type fjernsletning, du vil udføre. Tilbagetrækning sletter kun virksomhedsoplysninger, mens komplette sletninger gendanner enheden til fabriksindstillingerne.
4. Vælg **Ja for** at bekræfte. Indtil sletningen afsluttes, vises status for enhedshandlingen som Tilbagetrækning *afventer.*
    Når handlingen er fuldført, kan du ikke længere se mobilenheden på listen over administrerede enheder.

> [!NOTE]
> Firmadata kan ikke fjernes fra enheder, DER ER FORBUNDET til Azure AD. 

Du kan finde detaljerede oplysninger om effekten af handlingerne Tilbagetrækning og Sletning, herunder hvad der bevares, og hvad der slettes, i følgende dokumentation:

- [Fjern enheder ved at slette, trække dem tilbage eller manuelt fjerne tilmeldingen af enheden.](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe)
- [Sådan slettes kun virksomhedsdata fra Intune-administrerede apps](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [Slet alle data fra en macOS-enhed.](https://docs.microsoft.com/mem/intune/remote-actions/device-erase)