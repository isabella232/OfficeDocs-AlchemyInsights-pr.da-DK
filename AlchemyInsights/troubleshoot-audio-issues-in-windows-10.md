---
title: Fejlfinding i forbindelse med lydproblemer i Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3476"
- "9001463"
ms.openlocfilehash: f51fd233db5ae068e719f1cf3bc94a0dac82444f
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265010"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a>Fejlfinding i forbindelse med lydproblemer i Windows 10

**Kør fejlfindingsværktøjet til lyd**

1.  Åbn [indstillingerne for fejlfinding](ms-settings:troubleshoot).

2.  Vælg **Afafspilning af lyd** > **Kør fejlfindingsværktøjet**.

**Angive standardenheden**

Hvis du opretter forbindelse til en lydenhed ved hjælp af USB eller HDMI, skal du muligvis indstille enheden som standard:

1. Åbn **Start** > **lyd**, og vælg derefter **Lyd-** eller **Skift systemlyde** på listen over resultater.

2.  Vælg en enhed under fanen **Afspilning,** vælg **Angiv standard**, og vælg derefter **OK**.

**Kontrollere kabler, lydstyrke, højttalere og hovedtelefoner**

1. Kontroller højttaler- og hovedtelefontilslutninger for løse kabler, og sørg for, at de er tilsluttet det korrekte stik.

2. Kontroller strøm- og lydstyrkeniveauet, og prøv at skrue op for alle lydstyrkekontrolelementerne.

3. Nogle højttalere og apps har deres egne lydstyrkekontroller. du måske nødt til at tjekke dem alle for at sikre, at de er på de rigtige niveauer.

4. Prøv at oprette forbindelse ved hjælp af en anden USB-port.

**Bemærk:** Husk, at højttalerne muligvis ikke fungerer, når hovedtelefonerne er tilsluttet.

**Tjek Enhedshåndtering**

Sådan sikrer du dig, at chaufførerne er opdaterede:

1. Vælg **Start**, skriv **Enhedshåndtering**, og vælg derefter **Enhedshåndtering** på listen over resultater.

2. Vælg lydkortet under **Lyd-, video- og spilcontrollere,** åbn det, vælg fanen **Driver,** og vælg **Opdater driver**.

**Bemærk:** Hvis Windows ikke finder en ny driver, skal du kigge efter en på enhedsproducentens websted og følge deres instruktioner.

**Geninstallere driveren**

Hvis du ikke kan opdatere via Enhedshåndtering eller finde en ny driver på producentens websted, kan du prøve disse trin:

1. Højreklik (eller tryk og hold) lyddriveren i Enhedshåndtering, og vælg **Fjern**. Genstart enheden, og Windows forsøger at geninstallere driveren.

2. Hvis geninstallation af driveren ikke virker, kan du prøve at bruge den generiske lyddriver, der følger med Windows. Højreklik (eller tryk og hold) din lyddriver > **Opdater driversoftware** > **Gennemse min computer for driversoftware** > **Lad mig vælge fra en liste over enhedsdrivere på computeren,** vælge **High Definition Audio Device**, vælge **Næste**og følge vejledningen for at installere den.
