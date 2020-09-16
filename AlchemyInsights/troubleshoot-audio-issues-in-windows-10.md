---
title: Fejlfinding af lydproblemer i Windows 10
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
- "3476"
- "9001463"
ms.openlocfilehash: 88157f9c82bc970e989d47f5cf376b7ce485cb2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750301"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a>Fejlfinding af lydproblemer i Windows 10

**Kør fejlfindingsværktøjet lyd**

1.  Åbne [fejlfindingsindstillingerne](ms-settings:troubleshoot).

2.  Vælg **afspilning af lyd**  >  **Kør fejlfindingen**.

**Angive standardenheden**

Hvis du opretter forbindelse til en lydenhed med USB eller HDMI, skal du muligvis angive den pågældende enhed som standard:

1. Åbn **Start**  >  **lyd**, og vælg derefter **lyd** eller **Skift systemlyde** på listen over resultater.

2.  På fanen **afspilning** skal du vælge en enhed, vælge **Angiv standard**og derefter vælge **OK**.

**Kontrollér kabler, lydstyrke, højttalere og hovedtelefoner**

1. Kontrollér din højttaler og dine hovedtelefon forbindelser for løse kabler, og sørg for, at de er tilsluttet til det rigtige stik.

2. Kontrollér dine strøm-og lydstyrkeniveauer, og prøv at tænde for alle lydstyrkeindstillingerne.

3. Nogle højttalere og apps har deres egen lydstyrkekontrol. Du skal muligvis kontrollere dem alle for at sikre, at de er på de rigtige niveauer.

4. Prøv at oprette forbindelse ved hjælp af en anden USB-port.

**Bemærk**: Husk, at dine højttalere muligvis ikke fungerer, når hovedtelefoner er tilsluttet.

**Kontrollér Enhedshåndtering**

Sådan sikres det, at driverne er opdaterede:

1. Vælg **Start**, Skriv **Enhedshåndtering**, og vælg derefter **Enhedshåndtering** på listen over resultater.

2. Under **enheder til lydoptagelse, video og spil**skal du vælge dit lydkort, åbne det, vælge fanen **driver** og vælge **Opdater driver**.

**Bemærk**! hvis Windows ikke finder en ny driver, kan du søge efter en på enhedsproducentens websted og følge vejledningen.

**Geninstaller driveren**

Hvis du ikke kan opdatere via Enhedshåndtering eller finde en ny driver på producentens websted, kan du prøve disse trin:

1. I Enhedshåndtering skal du højreklikke (eller trykke og holde) på lyddriveren og vælge **Fjern**. Genstart din enhed, og Windows vil forsøge at geninstallere driveren.

2. Hvis geninstallation af driveren ikke virker, kan du prøve at bruge den generiske lyddriver, der følger med Windows. I Enhedshåndtering skal du højreklikke (eller trykke og holde) på lyddriveren > **Opdater driversoftware**  >  **Gennemse min computer for driversoftware**  >  **Lad mig vælge fra en liste over enhedsdrivere på min computer**, Vælg **næste**, og følg vejledningen for at installere den. **High Definition Audio Device**
