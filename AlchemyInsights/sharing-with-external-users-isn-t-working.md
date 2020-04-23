---
title: Deling med eksterne brugere fungerer ikke
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 285535d6144825f0935bf72579a483260c2f2bd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767243"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Løse problemer med at dele SharePoint-indhold med eksterne brugere

Sørg for, at ekstern deling er slået til for din organisation:
  
1. Gå til [ &amp; siden Med tilføjelsesprogrammet Tjenester i Microsoft 365 Administration](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), og klik på **Websteder**.
    
2. Sørg for, at indstillingen er slået til "Til". Hvis "Kun eksisterende eksterne brugere" er valgt, skal du kontrollere, at den eksterne bruger er angivet i Microsoft 365 Administration.
    
Sørg for, at ekstern deling er slået til for webstedet. For en klassisk gruppe af websteder:
  
1. Klik på **websteder**i venstre rude i den nye SharePoint Administration.
    
2. Vælg webstedet eller webstederne, og klik på **Deling**på båndet.
    
For et teamwebsted, der tilhører en Office 365-gruppe eller et kommunikationswebsted:
  
- Disse nye webstedstyper har samme delingsindstilling som indstillingen for hele organisationen, medmindre indstillingen for hele organisationen tillader deling af filer ved hjælp af links, der ikke kræver logon. I dette tilfælde tillader webstederne deling med nye og eksisterende eksterne brugere, der logger på. Hvis du vil ændre indstillingen for bestemte websteder, skal du bruge det nye SharePoint Administration eller PowerShell. [Få mere at vide](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Indstillingen for ekstern deling for et hvilket som helst websted kan være mere restriktiv end indstillingen for hele organisationen, men ikke mere eftergivende end indstillingen for hele organisationen. 
  

