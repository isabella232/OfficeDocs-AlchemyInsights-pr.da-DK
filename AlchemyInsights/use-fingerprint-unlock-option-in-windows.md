---
title: Brug mulighed for oplåsning af fingeraftryk i Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 8a5059c722c306ad79811140062cec7f52f31766
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588310"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Brug mulighed for oplåsning af fingeraftryk i Windows 10

**Aktiver Windows Hello-fingeraftryk**

Hvis du vil låse Windows 10 op ved hjælp af dit fingeraftryk, skal du konfigurere Windows Hello Fingerprint ved at tilføje (lade Windows lære at genkende) mindst én finger. 

1. Gå til **Indstillinger > konti > logonindstillinger** (eller klik [her](ms-settings:signinoptions?activationSource=GetHelp)). Tilgængelige logonindstillinger vises. Det kan f.eks. være:

    ![Indstillinger for logon.](media/sign-in-options.png)

2. Klik eller tryk på **Windows Hello Fingerprint**, og klik derefter på **Konfigurer**. Klik på Kom i **gang**i vinduet Windows Hello-konfiguration . Fingeraftrykssensoren aktiveres, og du bliver bedt om at placere fingeren på sensoren:

   ![Fingeraftrykssensor.](media/fingerprint-sensor.png)

3. Følg vejledningen, som vil bede dig om gentagne gange at scanne din finger. Når dette er færdigt, har du mulighed for at tilføje andre fingre, som du måske vil bruge til logon. Næste gang du logger på Windows 10, har du mulighed for at bruge dit fingeraftryk til at gøre det.

**Windows Hello Fingerprint er ikke tilgængelig som logonindstilling**

Hvis Windows Hello Fingerprint ikke vises som en indstilling i **logonindstillinger**, betyder det, at Windows ikke har kendskab til nogen fingeraftrykslæser/scanner, der er tilsluttet pc'en, eller at en systempolitik forhindrer brugen (hvis din pc f.eks. administreres af din arbejdsplads). Sådan foretages fejlfinding: 

1. Vælg knappen **Start** på proceslinjen, og søg efter **Enhedshåndtering**.

2. Klik eller tryk for at åbne **Enhedshåndtering**.

3. I Enhedshåndtering skal du udvide biometriske enheder ved at klikke på dens vinkel.

   ![Biometriske enheder.](media/biometric-devices.png)

4. Din fingeraftryksscanner skal være opført som en biometrisk enhed, f.eks.

   ![Biometriske enheder.](media/biometric-devices-expanded.png)

5. Hvis fingeraftryksscanneren ikke vises, og scanneren er integreret i pc'en, skal du gå til pc-producentens websted. I afsnittet teknisk support til pc-modellen skal du søge efter en Windows 10-driver til en scanner, du kan installere.

6. Hvis scanneren er adskilt fra pc'en (vedhæftet via USB), skal du gå til scannerproducentens websted for at finde og installere Windows 10-enhedsdriversoftware til den scannermodel, du har.
