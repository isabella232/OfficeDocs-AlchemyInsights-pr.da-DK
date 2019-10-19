---
title: Synkronisering af profiler
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/18/2019
ms.locfileid: "36554327"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Hvornår synkroniseres min profil med SharePoint-brugerprofilprogrammet?

SharePoint Online bruger Active Directory-tids jobbet til import af timer (AD import) til at importere brugere og grupper til brugerprofilprogrammet. 
  
1. AD import synkroniserer ændringer fra SharePoint Online-kataloglageret til brugerprofilprogrammet. Disse ændringer behandles i batches.
    
2. Timerjobbet køres, indtil ændringerne er synkroniseret.
    
> [!NOTE]
> Den tid, det tager jobbet at køre, afhænger af antallet af ændringer, der skal udføres. Et stort antal ændringer tager længere tid. Serviceniveauaftalen (SLA) fastslår, at en ændring af en bruger i SharePoint Online-mappen vil blive afspejlet i brugerprofilprogrammet inden for 24 timer. 
  
[Flere oplysninger om Brugerprofilsynkronisering i SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

