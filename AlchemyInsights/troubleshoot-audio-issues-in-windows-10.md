---
title: Fejlfinding af lydproblemer i Windows 10
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
- "3476"
- "9001463"
ms.openlocfilehash: 81a7f77bd6565c52ec9d752934a872e59cc11e89b90a646d17c3549d72e8a69f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039420"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a>Fejlfinding af lydproblemer i Windows 10

**Kør lydfejlfinding**

1.  Åbn indstillingerne [for fejlfinding.](ms-settings:troubleshoot)

2.  Vælg **Afspilning af lyd** Kør  >  **fejlfindingsværktøjet**.

**Angiv standardenheden**

Hvis du opretter forbindelse til en lydenhed ved hjælp af USB eller HDMI, skal du muligvis angive den pågældende enhed som standardenhed:

1. Åbn **Start**  >  **lyd**, og vælg derefter **Lyd** eller **Skift systemlyde** på listen over resultater.

2.  På fanen **Afspilning** skal du vælge en enhed, **vælge Angiv standard** og derefter vælge **OK**.

**Tjek kabler, lydstyrke, højttalere og hovedtelefoner**

1. Kontrollér dine højttaler- og hovedtelefonforbindelser for løse kabler, og sørg for, at de er forbundet til det rigtige stik.

2. Kontrollér strøm og lydstyrkeniveauer, og prøv at skrue op for alle lydstyrkeknapper.

3. Nogle højttalere og apps har deres egne lydstyrkeknapper. skal du muligvis kontrollere dem alle for at sikre dig, at de er på de rigtige niveauer.

4. Prøv at tilslutte ved hjælp af en anden USB-port.

**Bemærk:** Husk, at dine højttalere muligvis ikke fungerer, når hovedtelefonerne er tilsluttet.

**Kontrollér Enhedshåndtering**

Sådan sikrer du, at driverne er opdaterede:

1. Vælg **Start**, skriv **Enhedshåndtering**, og vælg **derefter Enhedshåndtering** på listen over resultater.

2. Under **Lyd, video og spilcontrollere** skal du vælge dit lydkort, åbne det, vælge fanen **Driver** og vælge **Opdater driver**.

**Bemærk!** Hvis Windows finder en ny driver, skal du søge efter en på enhedsproducentens websted og følge instruktionerne.

**Geninstaller driveren**

Hvis du ikke kan opdatere via Enhedshåndtering eller finde en ny driver på producentens websted, kan du prøve disse trin:

1. I Enhedshåndtering skal du højreklikke (eller trykke og holde nede) på lyddriveren og vælge **Fjern.** Genstart enheden, så Windows forsøge at geninstallere driveren.

2. Hvis det ikke virker at geninstallere driveren, kan du prøve at bruge den generiske lyddriver, der leveres Windows. I Enhedshåndtering skal du højreklikke (eller trykke og holde) på din lyddriver > Opdater **driversoftware** Gennemse computeren efter driversoftware Lad mig vælge på en liste over enhedsdrivere på computeren , vælg Lydenhed med HD , vælg Næste , og følg vejledningen for at installere  >    >  den.  
