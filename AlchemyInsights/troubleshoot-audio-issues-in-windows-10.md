---
title: Fejlfinding af lydproblemer i Windows 10
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
ms.openlocfilehash: 46b23f97c2e682258224dc95e7a76b1201991828
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796043"
---
# <a name="troubleshooting-audio-problems-in-windows-10"></a>Fejlfinding af lydproblemer i Windows 10

**Kør fejlfindingsværktøjet lyd**

Lydfejlfinding kan muligvis løse lydproblemerne automatisk: 

1. Vælg **Start**, Skriv **fejlfinding**, og vælg derefter **fejlfinding** på listen over resultater. 
2. Vælg **afspilning af lyd** > **Kør fejlfindingsværktøjet**.

**Kontrollér kabler, lydstyrke, højttalere og hovedtelefoner**

- Kontrollér dine højttaler-og hovedtelefon tilslutninger for løse kabler, og sørg for, at de er sluttet til det rigtige stik.
- Kontrollér dine strøm-og lydstyrkeniveauer, og prøv at slå alle lydstyrkekontrollerne op.
- Nogle højttalere og apps har deres egne lydstyrke Kontroller, og du skal muligvis kontrollere dem alle for at sikre, at de er på de rigtige niveauer.
- Prøv at oprette forbindelse ved hjælp af en anden USB-port.
- **Bemærk:** Husk, at dine højttalere muligvis ikke fungerer, når hovedtelefonerne er tilsluttet.

**Kontroller Enhedshåndtering**

Sådan sikrer du dig, at driverne er opdateret:

- Vælg **Start**, Skriv **Enhedshåndtering**, og vælg derefter **Enhedshåndtering** på listen over resultater.

2. Vælg lydkortet under **enheder til lyd, video og spil**, Åbn det, Vælg fanen **driver** , og vælg **Opdater driver**. 

**Bemærk:** Hvis Windows ikke finder en ny driver, skal du søge efter en på enhedsproducentens websted og følge instruktionerne.

**Geninstallere driveren**

Hvis du ikke kan opdatere via Enhedshåndtering eller finde en ny driver på producentens websted, skal du prøve disse trin: 

1. Højreklik (eller tryk og hold) på lyddriveren i Enhedshåndtering, og vælg **Fjern**. Genstart enheden, og Windows vil forsøge at geninstallere driveren.

2. Hvis geninstallation af driveren ikke virker, kan du prøve at bruge den generiske lyddriver, der følger med Windows. I Enhedshåndtering skal du højreklikke (eller trykke og holde) på din lyddriver **> opdatere driver software** > **Gennemse min computer for driver software** > **Lad mig vælge fra en liste over enhedsdrivere på min computer**, Vælg **High Definition Audio Device**, Vælg **næste**, og følg instruktionerne for at installere den.

**Angive standardenheden**

Hvis du opretter forbindelse til en lydenhed ved hjælp af USB eller HDMI, skal du muligvis indstille enheden som standard: 

1. Vælg **Start**, Skriv **lyd**, og vælg derefter **lyd** eller **Skift systemlyde** på listen over resultater.

2. Vælg en enhed under fanen **afspilning** , Vælg **Angiv standard**, og vælg derefter **OK**.

