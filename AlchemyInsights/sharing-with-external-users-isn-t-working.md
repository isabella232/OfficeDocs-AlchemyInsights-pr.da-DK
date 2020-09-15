---
title: Deling med eksterne brugere fungerer ikke
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691569"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Løs problemer med at dele SharePoint-indhold med eksterne brugere

Sørg for, at ekstern deling er slået til for din organisation:
  
1. Gå til [siden tjenester &amp; -tilføjelsesprogrammer i Microsoft 365 administration](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), og klik på **websteder**.
    
2. Sørg for, at indstillingen er slået til "slået til." Hvis "kun eksisterende eksterne brugere" er markeret, skal du kontrollere, at den eksterne bruger er angivet i Microsoft 365 administration.
    
Sørg for, at ekstern deling er slået til for webstedet. For en klassisk gruppe af websteder:
  
1. Klik på **websteder**i venstre rude i den nye SharePoint administration-ressource.
    
2. Vælg webstedet eller webstederne, og klik på **deling**på båndet.
    
For et teamwebsted, der tilhører en Microsoft 365-gruppe eller et kommunikationswebsted:
  
- Disse nye websteds typer har samme indstilling som indstillingen for hele organisationen, medmindre indstillingen for hele organisationen gør det muligt at dele filer ved hjælp af links, der ikke kræver logon. I dette tilfælde tillader webstederne deling med nye og eksisterende eksterne brugere, der logger på. Hvis du vil ændre indstillingen for bestemte websteder, skal du bruge den nye SharePoint administration eller PowerShell. [Få mere at vide](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Indstillingen for ekstern deling for ethvert websted kan være mere restriktivt end din indstilling for hele organisationen, men det er ikke mere tilskrivende end indstillingen for hele organisationen. 
  

