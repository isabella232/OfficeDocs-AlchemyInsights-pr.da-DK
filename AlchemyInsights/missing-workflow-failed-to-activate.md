---
title: Manglende arbejdsprocessen kunne ikke aktiveres
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: ce088227a3206fa05b99331fdb022fbe4886203f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/12/2019
ms.locfileid: "29917562"
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
  

