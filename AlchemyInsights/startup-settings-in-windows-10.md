---
title: Startindstillinger i Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: b4854944d8cbd9bd83fdea609007c15d39c8eb75
ms.sourcegitcommit: c55eea624d960d2dd17ac4aa5a4c23e34e6443b8
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/04/2020
ms.locfileid: "42408969"
---
# <a name="startup-settings-in-windows-10"></a>Startindstillinger i Windows 10

**Ændre, hvilke apps der kører automatisk ved start**

1. Gå til [Indstillinger > Apps > Start](ms-settings:startupapps?activationSource=GetHelp).

2. Sørg for, at alle apps, du vil køre ved start, er **slået**til .

**Tilføje en app for at køre automatisk ved start**

1. Klik eller tryk på **Start,** og find den app, du vil køre ved start.

2. Højreklik på appen, klik på **Mere**, og klik derefter på **Åbn filplacering**. Dette åbner den placering, hvor genvejen til appen gemmes. Hvis der ikke er nogen indstilling for Placering af Åbn fil, betyder det, at appen ikke kan køre ved start.

3. Når filplaceringen er åben, skal du trykke på **Windows-tasten + R**, skrive **shell:startup**og derefter klikke på **OK**. Derved åbnes mappen Start.

4. Kopiér og indsæt genvejen til appen fra filplaceringen i mappen Start.

**Avancerede startindstillinger (herunder fejlsikret tilstand, UEFI-indstillinger og opstart fra en anden enhed)**

1. Gem dit arbejde, og luk alle åbne dokumenter, da disse trin genstarter pc'en.

2. Gå til [Indstillinger > Opdatering & Genoprettelse > sikkerhedsgendannelse](ms-settings:recovery?activationSource=GetHelp).

3. Klik på **Genstart nu**under **Avanceret start**. 

4. Når din pc er genstartet til skærmbilledet Vælg en indstilling:

    - Hvis du vil starte fra en enhed som et USB-drev, skal du klikke på **Brug en enhed**.

    - Hvis du vil angive UEFI-indstillingerne (også kaldet BIOS-opsætning), skal du klikke **på Fejlfinding > Avancerede indstillinger > UEFI-firmwareindstillinger**. 

    - Hvis du vil angive fejlsikret tilstand eller ændre avancerede startindstillinger, skal du klikke på **Fejlfinding > Avancerede indstillinger > Startindstillinger**og derefter klikke på **Genstart**. Du kan blive bedt om at angive [bitlockergenoprettelsesnøglen](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key). Når pc'en er genstartet igen, skal du klikke på den startindstilling, du vil bruge.