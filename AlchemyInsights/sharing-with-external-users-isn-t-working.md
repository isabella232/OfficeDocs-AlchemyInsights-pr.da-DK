---
title: Deling med eksterne brugere fungerer ikke
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 305b3891e6c83e27b5c55c13757640e6e9d51a81
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/15/2019
ms.locfileid: "28283066"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Løse problemer med Deling af SharePoint-indhold med eksterne brugere

Sørg for, at eksterne deling er aktiveret for organisationen:
  
1. Gå til den [Services &amp; tilføjelsesprogrammer side i Office 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), og klik på **websteder**.
    
2. Kontroller, at indstillingen er slået til "On". Hvis "Kun eksisterende eksterne brugere" er valgt, skal du kontrollere den eksterne bruger er angivet i Office 365 admin center.
    
Kontroller, at Deling af den eksterne aktiveret for webstedet. For en klassisk websteder:
  
1. Klik på **grupper af websteder**i den klassiske SharePoint admin center, i venstre rude.
    
2. Vælg den eller de websteder, og på båndet, skal du klikke på **Deling**.
    
For et websted for team, der tilhører en gruppe af Office 365, eller et kommunikationswebsted:
  
- Disse nye websted har den samme deling indstilling som den globale indstilling, medmindre den globale indstilling tillader deling af filer ved hjælp af hyperlinks, der ikke kræver logon. I dette tilfælde kan webstederne deler med nye og eksisterende eksterne brugere, der logger på. Hvis du vil ændre indstillingen for bestemte websteder, ved at bruge nye SharePoint admin center (eksempel) eller PowerShell. [Få mere at vide](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Indstillingen for eksterne deling for ethvert websted kan være mere restriktive end den globale indstilling, men ikke mere lempelige end den globale indstilling. 
  

