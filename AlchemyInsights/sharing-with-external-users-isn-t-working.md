---
title: Deling med eksterne brugere virker ikke
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
ms.openlocfilehash: 53f6fd009d3dab3cd66d33d9cd248201219caa1605c7a4e7758a5a8d720f68c2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53910360"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Løs problemer med SharePoint indhold med eksterne brugere

Sørg for, at ekstern deling er aktiveret for din organisation:
  
1. Gå til [siden Tjenester for &amp; tilføjelsesprogrammet Tjenester i Microsoft 365 Administration](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), og klik på **Websteder**.
    
2. Sørg for, at indstillingen er slået til "Til". Hvis "Kun eksisterende eksterne brugere" er markeret, skal du kontrollere, at den eksterne bruger er angivet i Microsoft 365 Administration.
    
Sørg for, at ekstern deling er slået til for webstedet. For en klassisk gruppe af websteder:
  
1. I den nye SharePoint Administration skal du i venstre rude klikke på **websteder**.
    
2. Vælg webstedet eller webstederne, og klik på Deling på **båndet.**
    
For et teamwebsted, der tilhører en Microsoft 365 gruppe eller et kommunikationswebsted:
  
- Disse nye webstedstyper har samme indstilling for deling som indstillingen for hele organisationen, medmindre indstillingen for hele organisationen tillader deling af filer ved hjælp af links, der ikke kræver, at du logger på. I dette tilfælde tillader webstederne deling med nye og eksisterende eksterne brugere, der logger på. Hvis du vil ændre indstillingen for bestemte websteder, skal du SharePoint administration eller PowerShell. [Få mere at vide](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Indstillingen til ekstern deling for et websted kan være mere restriktiv end indstillingen for hele organisationen, men den kan ikke være mere restriktiv end indstillingen for hele organisationen. 
  

