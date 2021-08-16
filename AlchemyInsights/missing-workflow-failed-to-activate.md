---
title: Manglende arbejdsproces kunne ikke aktiveres
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: d703e87f355f05bf4a1d71e5daddce96db988380bb48accc81c95f1ba91fbb2b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54065422"
---
# <a name="missing-workflow-failed-to-activate"></a>Manglende arbejdsproces kunne ikke aktiveres

I en Microsoft SharePoint gruppe af websteder kan du ikke føje en arbejdsproces, der kan genbruges globalt (f.eks. "Godkendelse – SharePoint 2010") til en liste eller et bibliotek.
  
Du kan løse dette problem ved at følge disse trin: 
  
1. Åbn rodwebstedet for gruppen af websteder i SharePoint Designer 2013.
  
2. Under **Webstedsobjekter** skal du **vælge Arbejdsprocesser**. 
  
3. I sektionen **Ny** på båndet **Arbejdsprocesser skal** du vælge **Genanvendelig arbejdsproces.** 
  
4. I formularen **Opret genanvendelige arbejdsprocesser** skal du skrive navnet ** *Repair2010* **. Under **Platformstype** skal du klikke **SharePoint 2010-arbejdsproces** og derefter klikke på **OK.** 
  
1. I sektionen **Gem** på båndet Arbejdsproces **skal** du vælge **Publicer**. 
  
2. I sektionen **Administrer** på båndet **Arbejdsproces** skal du **vælge Publicer globalt.** Vælg OK i bekræftelsesdialogboksen, der **vises.** 
  
3. Find rodwebstedet for gruppen af websteder i en webbrowser, og få derefter adgang til funktionerne **Indstillinger gruppen** \> **af websteder**. Slå derefter funktionen **Arbejdsprocesser** til eller fra: 
  
· Hvis funktionen er *aktiveret, skal du* klikke på **Deaktiver og** derefter klikke på **Aktivér.** 
  
· Hvis funktionen er  *deaktiveret, skal du*  klikke på **Aktivér**. 
  
Du kan finde flere oplysninger i følgende [artikel.](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)
  

