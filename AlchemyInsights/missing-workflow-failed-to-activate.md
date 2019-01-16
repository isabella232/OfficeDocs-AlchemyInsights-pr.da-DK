---
title: Manglende arbejdsprocessen kunne ikke aktiveres
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 33b92c2cae1f641b0cd88c82fd4ae5e8632d76c2
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/15/2019
ms.locfileid: "28283380"
---
# <a name="missing-workflow-failed-to-activate"></a>Manglende arbejdsprocessen kunne ikke aktiveres

I et Microsoft SharePoint-websteder, kan ikke du føje et globalt genbrugelig arbejdsproces (f.eks "godkendelse - SharePoint 2010") til en liste eller et bibliotek.
  
Du kan løse dette problem ved at følge disse trin: 
  
1. Åbn rod-websted for gruppen af websteder i SharePoint Designer 2013.
  
2. Vælg **arbejdsprocesser**under **Objekter**. 
  
3. Vælg **Arbejdsproces, kan genbruges**i afsnittet **Ny** i båndet **arbejdsprocesser** . 
  
4. Angiv navnet formularen **Opret genanvendelig arbejdsproces** ** *Repair2010* **. Klik på **SharePoint 2010-arbejdsproces**til **Platform er af typen**, og klik derefter på **OK**. 
  
1. Vælg **Udgiv**i afsnittet **Gem** i **arbejdsproces** -båndet. 
  
2. Vælg **Udgiv globalt**i afsnittet **Manage** i **arbejdsproces** -båndet. Klik på **OK**i bekræftelsesdialogboksen. 
  
3. Find på rod-webstedet for gruppen af websteder i en webbrowser, og derefter få adgang til **Indstillinger for websted** \> **Funktioner på gruppen af websteder**. Slå derefter funktionen **arbejdsprocesser** : 
  
· Hvis funktionen er *aktiveret* , skal du klikke på **Deaktiver,** og klik derefter på **Aktiver**. 
  
· Hvis funktionen er *deaktiveret* , skal du klikke på **Aktiver**. 
  
Se følgende [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)for at få yderligere oplysninger.
  

