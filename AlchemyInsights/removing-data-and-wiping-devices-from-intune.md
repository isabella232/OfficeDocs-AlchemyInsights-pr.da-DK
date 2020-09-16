---
title: Fjerne data og slette enheder fra Intune
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
ms.openlocfilehash: 24330dffb38be14dd369960ff86d4650d60c55ec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47701277"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Fjerne data og slette enheder fra Intune

Aflevering af enheden og fjernhandlinger til sletning af enheder kan bruges til at fjerne virksomhedsdata, der administreres af Intune, eller til at udføre en Fabriks nulstilling og sætte enheden tilbage til standardindstillingerne.

1. Log på Microsoft 365-Enhedsadministration, og gå til **enheder**på  >  **alle enheder**.
2. Vælg den enhed, du vil slette.
3. Vælg den type Fjern sletning, du vil udføre. Tilbagetrækning sletter kun organisationsoplysninger, mens alle sletninger gendanner enheden til fabriksindstillingerne.
4. Vælg **Ja** for at bekræfte. Indtil sletningen er fuldført, vises status for enheds handlingen som afventer tilbagetrækning.</br>
    Når handlingen er fuldført, kan du ikke længere se mobilenheden på listen over administrerede enheder.

**Bemærk!** Firmadata kan ikke fjernes fra enheder, der er knyttet til Azure AD.

Hvis du vil have detaljerede oplysninger om effekten af aftræks-og slette handlingerne, herunder hvad der bevares, og hvad der slettes, skal du se [fjerne enheder ved hjælp af slet, Fjern eller Fjern registreringen af enheden manuelt](https://docs.microsoft.com/intune/devices-wipe).

Hvis du vil slette alle data fra en macOS-enhed, skal du se [Slet alle data fra en macOS-enhed](https://docs.microsoft.com/intune/device-erase).