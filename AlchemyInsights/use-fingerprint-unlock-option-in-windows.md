---
title: Brug indstillingen oplåsning af fingeraftryk i Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795238"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Brug indstillingen oplåsning af fingeraftryk i Windows 10

**Aktivér Windows Hello-fingeraftryk**

Hvis du vil låse Windows 10 op ved hjælp af dit fingeraftryk, skal du konfigurere Windows Hello-fingeraftryk ved at tilføje (lade Windows lære at genkende) mindst én finger. 

1. Gå til **indstillinger > konti > indstillinger for logon** (eller klik [her](ms-settings:signinoptions?activationSource=GetHelp)). Tilgængelige logonindstillinger vises. Det kan f.eks. være:

    ![Logonindstillinger.](media/sign-in-options.png)

2. Klik eller tryk på **Windows Hello-fingeraftryk**, og klik derefter på **Konfigurer**. I vinduet Windows Hello-konfiguration skal du klikke på **Introduktion**. Fingeraftrykssensoren aktiveres, og du bliver bedt om at sætte fingeren på sensoren:

   ![Fingeraftrykssensor.](media/fingerprint-sensor.png)

3. Følg vejledningen, så du bliver bedt om at scanne din finger gentagne gange. Når dette er gjort, har du mulighed for at tilføje andre fingre, som du vil bruge til at logge på. Næste gang du logger på Windows 10, får du mulighed for at bruge dit fingeraftryk til at gøre det.

**Windows Hello-fingeraftryk er ikke tilgængelig som en logonindstilling**

Hvis Windows Hello-fingeraftryk ikke vises som en valgmulighed i **Indstillinger for logon**, betyder det, at Windows ikke kender en fingeraftrykslæser/scanner, der er tilsluttet din pc, eller at en systempolitik forhindrer dens brug (hvis for eksempel din pc administreres af din arbejdsplads). Sådan foretager du fejlfinding: 

1. Vælg knappen **Start** på proceslinjen, og Søg efter **Enhedshåndtering**.

2. Klik eller tryk for at åbne **Enhedshåndtering**.

3. Udvid biometriske enheder i Enhedshåndtering ved at klikke på dens vinkel.

   ![Biometriske enheder.](media/biometric-devices.png)

4. Din fingeraftryksscanner skal være angivet som en biometrisk enhed, såsom Synaptics WBDI-scanneren:

   ![Biometriske enheder.](media/biometric-devices-expanded.png)

5. Hvis din fingeraftryksscanner ikke vises, og scanneren er integreret i din PC, skal du gå til PC-producentens websted. I afsnittet teknisk support for din PC-model skal du søge efter en Windows 10-driver til en scanner, som du kan installere.

6. Hvis scanneren er adskilt fra pc'en (tilsluttet via USB), skal du gå til scanner producentens websted for at finde og installere Windows 10-enhedsdriversoftware til den scannermodel, du har.
