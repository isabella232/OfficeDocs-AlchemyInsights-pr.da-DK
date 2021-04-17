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
ms.openlocfilehash: 1bafc97b2ab1394087d2451d73168a29267d64ab
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833285"
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

**Bemærk!** Hvis Windows ikke finder en ny driver, skal du søge efter en på webstedet for enhedsproducenten og følge instruktionerne.

**Geninstaller driveren**

Hvis du ikke kan opdatere via Enhedshåndtering eller finde en ny driver på producentens websted, kan du prøve disse trin:

1. I Enhedshåndtering skal du højreklikke (eller trykke og holde nede) på lyddriveren og vælge **Fjern.** Genstart enheden, så forsøger Windows at geninstallere driveren.

2. Hvis det ikke virker at geninstallere driveren, kan du prøve at bruge den generiske lyddriver, der leveres med Windows. I Enhedshåndtering skal du højreklikke (eller trykke og holde) på din lyddriver > Opdater **driversoftware** Gennemse computeren efter driversoftware Lad mig vælge på en liste over enhedsdrivere på computeren , vælg Lydenhed med HD , vælg Næste , og følg vejledningen for at installere  >    >  den.  
