---
title: Diagram viser et andet antal poster i gitter
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
ms.openlocfilehash: e499a439e7cf7e9ecbb6566f9f089f3b7b82f48e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47793752"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a>Diagram viser et andet antal poster i gitter

**Symptom**

For diagram på dashboardsiden, når du klikker på diagram "..." og klik på "Vis poster", skal du gå til gitter side for at få vist alle posterne. Nogle gange ændres antallet af poster.

**Kræve**

Dette skyldes forskellen mellem visningen af diagrammet på den oprindelige dashboardside og diagrammet på gitter startsiden.  

**Løsning**

1. Markér visningen på den oprindelige side og visningen i gitteret for at se, om de er forskellige.
2. Du kan ændre visningen i gitteret, så det svarer til visningen på den oprindelige side.
3. Hvis den korrekte visning ikke kan findes, betyder det normalt, at visningen ikke er aktiveret i app designer.
4. Gå til App designer for den bestemte app, Vælg objektet og dens visninger, Markér den visning, du vil aktivere, gemme, publicere og lukke.
5. Opdater siden.