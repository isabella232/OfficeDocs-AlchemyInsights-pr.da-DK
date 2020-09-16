---
title: Startindstillinger i Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: e49faca66785c6611dda702a381c39cdb10884f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751129"
---
# <a name="startup-settings-in-windows-10"></a>Startindstillinger i Windows 10

**Ændre, hvilke apps der kører automatisk ved start**

1. Gå til [indstillinger > Apps > start](ms-settings:startupapps?activationSource=GetHelp).

2. Kontrollér, at alle de apps, du vil køre ved opstart, er slået **til.**

**Tilføj en app til at køre automatisk ved start**

1. Klik eller tryk på **Start** , og Find den app, du vil køre ved opstart.

2. Højreklik på appen, klik på **flere**, og klik derefter på **Åbn filplacering**. Dette åbner den placering, hvor genvejen til appen er gemt. Hvis der ikke er nogen indstilling for åben filplacering, betyder det, at appen ikke kan køre ved start.

3. Når filplaceringen er åben, skal du trykke på **Windows-tasten + R**, skrive **Shell: Start**og derefter klikke på **OK**. Dette åbner mappen Start.

4. Kopiér og Indsæt genvejen til appen fra filplaceringen til mappen Start.

**Avancerede startindstillinger (herunder fejlsikret tilstand, UEFI-indstillinger og opstart fra en anden enhed)**

1. Gem dit arbejde, og Luk alle åbne dokumenter, da disse trin vil genstarte din PC.

2. Gå til [indstillinger > opdater & sikkerhed > genoprettelse](ms-settings:recovery?activationSource=GetHelp).

3. Under **Avanceret start**skal du klikke på **Genstart nu**. 

4. Når din PC genstarter på skærmbilledet Vælg en indstilling:

    - Hvis du vil starte fra en enhed som et USB-drev, skal du klikke på **Brug en enhed**.

    - Hvis du vil angive UEFI-indstillingerne (også kaldet BIOS-konfiguration), skal du klikke på **fejlfinding > avancerede indstillinger > UEFI-firmware indstillinger**. 

    - Hvis du vil angive fejlsikret tilstand eller ændre avancerede startindstillinger, skal du klikke på **fejlfinding > avancerede indstillinger > startindstillinger**og derefter klikke på **Genstart**. Du bliver muligvis bedt om at angive din [BitLocker-genoprettelsesnøgle](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key). Når din PC genstartes igen, skal du klikke på den startindstilling, du vil bruge.