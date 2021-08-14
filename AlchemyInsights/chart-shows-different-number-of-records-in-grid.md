---
title: Diagrammet viser forskellige antal poster i gitteret
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: 68ba6caf602a5cf60e2c96c80703f19dd07c3b6430c2a66f40fea4a2f3d06e75
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53950074"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a>Diagrammet viser forskellige antal poster i gitteret

**Symptom**

For diagram på dashboardside, når du klikker på diagrammet "..." og klikker på "Vis poster", navigerer du til gittersiden for at få vist alle posterne. Nogle gange ændres antallet af poster.

**Årsag**

Dette skyldes de forskellige visninger mellem diagrammet på den oprindelige dashboardside og diagrammet på gitterets startside.  

**Løsning**

1. Kontrollér visningen fra den oprindelige side og visningen i gitteret for at se, om de er forskellige.
2. Rediger visningen i gitteret, så den passer til visningen på den oprindelige side.
3. Hvis den korrekte visning ikke kan findes, betyder det som regel, at visningen ikke er aktiveret i appdesigneren.
4. Gå til Appdesigner for den specifikke app, vælg enheden og dens visninger, kontrollér den visning, du vil aktivere, gemme, publicere og lukke.
5. Opdater siden.