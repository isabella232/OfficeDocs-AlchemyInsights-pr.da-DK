---
title: Diagram viser forskellige antal poster i gitter
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: 3d0be28c783bb129d05484565c6c2a56ac5e0acf
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439003"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a>Diagram viser forskellige antal poster i gitter

**Symptom**

For diagram på dashboard side, når du klikker på diagrammet "..." og klik på "Vis poster", skal du navigere til gittersiden for at se alle posterne. Nogle gange ændres antallet af poster.

**Forårsage**

Dette skyldes forskellen mellem visningerne mellem diagrammet på den oprindelige dashboardside og diagrammet på gitterets startside.  

**Løsning**

1. Kontroller visningen fra den oprindelige side og visningen i gitteret for at se, om de er forskellige.
2. Rediger visningen i gitteret, så den svarer til visningen på den oprindelige side.
3. Hvis den korrekte visning ikke kan findes, betyder det normalt, at visningen ikke er aktiveret i appdesigner.
4. Gå til appdesigner for den specifikke app, vælg objektet og dets visninger, markér den visning, du vil aktivere, gemme, udgive og lukke.
5. Opdater siden.