---
title: Deling med eksterne brugere fungerer ikke
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 69e290e5a13f40ad045086791189a7d0af88240b
ms.sourcegitcommit: 228c986911ecf73217116a5d1fdcd2e89362774e
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/09/2019
ms.locfileid: "31747592"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Løse problemer med Deling af SharePoint-indhold med eksterne brugere

Sørg for, at eksterne deling er aktiveret for organisationen:
  
1. Gå til den [Services &amp; tilføjelsesprogrammer side i Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), og klik på **websteder**.
    
2. Kontroller, at indstillingen er slået til "On". Hvis "Kun eksisterende eksterne brugere" er valgt, skal du kontrollere den eksterne bruger er angivet i Microsoft 365 admin center.
    
Kontroller, at Deling af den eksterne aktiveret for webstedet. For en klassisk websteder:
  
1. Klik på **websteder**i det nye center på SharePoint-administrator i venstre rude.
    
2. Vælg den eller de websteder, og på båndet, skal du klikke på **Deling**.
    
For et websted for team, der tilhører en gruppe af Office 365, eller et kommunikationswebsted:
  
- Disse nye websted har den samme deling indstilling som den globale indstilling, medmindre den globale indstilling tillader deling af filer ved hjælp af hyperlinks, der ikke kræver logon. I dette tilfælde kan webstederne deler med nye og eksisterende eksterne brugere, der logger på. Hvis du vil ændre indstillingen for bestemte websteder, ved at bruge nye SharePoint Administration center eller PowerShell. [Få mere at vide](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Indstillingen for eksterne deling for ethvert websted kan være mere restriktive end den globale indstilling, men ikke mere lempelige end den globale indstilling. 
  

