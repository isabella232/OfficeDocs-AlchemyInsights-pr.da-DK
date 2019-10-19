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
ms.openlocfilehash: d4c8fc75ff8db2319b88a20bea9b3ee661f2e36e
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/18/2019
ms.locfileid: "36502225"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Løs problemer med deling af SharePoint-indhold med eksterne brugere

Sørg for, at ekstern deling er slået til for din organisation:
  
1. Gå til [siden med &amp; tilføjelsesprogrammer til tjenester i Microsoft 365 administration](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), og klik på **websteder**.
    
2. Sørg for, at indstillingen er slået til "til". Hvis "kun eksisterende eksterne brugere" er valgt, skal du kontrollere, at den eksterne bruger er angivet i Microsoft 365 administration.
    
Sørg for, at ekstern deling det er slået til for webstedet. For en klassisk gruppe af websteder:
  
1. Klik på **websteder**i den venstre rude i det nye SharePoint-Administrationscenter.
    
2. Vælg webstedet eller webstederne, og klik på **deling**på båndet.
    
For et teamwebsted, der tilhører en Office 365-gruppe, eller et kommunikationswebsted:
  
- Disse nye webstedstyper har samme delingsindstilling som indstillingen for hele organisationen, medmindre indstillingen for hele organisationen tillader deling af filer ved hjælp af links, der ikke kræver logon. I dette tilfælde tillader webstederne deling med nye og eksisterende eksterne brugere, der logger på. Hvis du vil ændre indstillingen for bestemte websteder, skal du bruge det nye SharePoint-Administrationscenter eller PowerShell. [Læs mere](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Den eksterne delingsindstilling for et hvilket som helst websted kan være mere restriktiv end organisationens indstillinger, men ikke mere eftergivende end den globale indstilling. 
  

