---
title: Kan ikke tilføje standard 2010 godkendelsesforløb
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2060c9a1-e714-4d93-925e-629c82c35986
ms.openlocfilehash: 758b0339b842478f9609eb716b5b4ddab6579c80
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/24/2019
ms.locfileid: "29463691"
---
# <a name="cant-add-default-2010-approval-workflow"></a>Kan ikke tilføje standard 2010 godkendelsesforløb

I et Microsoft SharePoint-websteder, kan ikke du føje et globalt genbrugelig arbejdsproces (f.eks "godkendelse - SharePoint 2010") til en liste eller et bibliotek.
  
Du kan løse dette problem ved at følge disse trin: 
  
1. Åbn rod-websted for gruppen af websteder i SharePoint Designer 2013.
  
2. Vælg **arbejdsprocesser**under **Objekter**. 
  
3. Vælg **Arbejdsproces, kan genbruges**i afsnittet **Ny** i båndet **arbejdsprocesser** . 
  
4. Angiv navnet formularen **Opret genanvendelig arbejdsproces** * **Repair2010***. Vælg **Arbejdsgange i SharePoint 2010** **Platform er af typen**, og klik derefter på **OK**. 
  
5. Vælg **Udgiv**i afsnittet **Gem** i **arbejdsproces** -båndet. 
  
6. Vælg **Udgiv globalt**i afsnittet **Manage** i **arbejdsproces** -båndet. Klik på **OK**i bekræftelsesdialogboksen. 
  
7. Find på rod-webstedet for gruppen af websteder i en webbrowser, og derefter få adgang til **Indstillinger for websted** \> **Funktioner på gruppen af websteder**. Slå derefter funktionen **arbejdsprocesser** : 
  
· Hvis funktionen er *aktiveret* , skal du klikke på **Deaktiver,** og klik derefter på **Aktiver**. 
  
· Hvis funktionen er *deaktiveret* , skal du klikke på **Aktiver**. 
  
Se følgende [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)for at få yderligere oplysninger.
  

