---
title: Startindstillinger i Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: 6dfae58a398db088ba00d9c2ea9788bab929ccc1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51828146"
---
# <a name="startup-settings-in-windows-10"></a>Startindstillinger i Windows 10

**Ændre, hvilke apps der køres automatisk ved start**

1. Gå til [Indstillinger > Apps > Start.](ms-settings:startupapps?activationSource=GetHelp)

2. Kontrollér, at alle apps, du vil køre ved start, er slået **Til.**

**Tilføj en app, der skal køre automatisk ved start**

1. Klik eller tryk **på Start,** og find den app, du vil køre ved start.

2. Højreklik på appen, klik på **Mere**, og klik derefter på **Åbn filplacering**. Dette åbner den placering, hvor genvejen til appen er gemt. Hvis der ikke er nogen indstilling for Åbn filplacering, betyder det, at appen ikke kan køre ved start.

3. Åbn filplaceringen, tryk på **Windows-tasten + R**, skriv **shell:startup**, og klik derefter på **OK**. Derved åbnes mappen Start.

4. Kopiér og indsæt genvejen til appen fra filplaceringen til mappen Start.

**Avancerede startindstillinger (herunder Fejlsikret tilstand, UEFI-indstillinger og start fra en anden enhed)**

1. Gem dit arbejde, og luk alle åbne dokumenter, da disse trin genstarter din pc.

2. Gå til [Indstillinger > opdatering & > genoprettelse.](ms-settings:recovery?activationSource=GetHelp)

3. Klik **på Genstart** nu under **Avanceret start.** 

4. Når pc'en genstarter, skal du gå til skærmbilledet Vælg en indstilling:

    - Hvis du vil starte fra en enhed som f.eks. et USB-drev, skal **du klikke på Brug en enhed**.

    - Hvis du vil angive UEFI-indstillingerne (nogle gange kaldetFUNKTIONER), skal du klikke på **Fejlfinding > avancerede indstillinger > UEFI-firmwareindstillinger.** 

    - Hvis du vil skifte fejlsikret tilstand eller ændre de avancerede startindstillinger, skal du klikke **på Fejlfinding >** avancerede > Indstillinger for start og derefter klikke på **Genstart.** Du bliver muligvis bedt om at angive [bitLocker-genoprettelsesnøglen](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key). Når pc'en genstarter igen, skal du klikke på den startindstilling, du vil bruge.