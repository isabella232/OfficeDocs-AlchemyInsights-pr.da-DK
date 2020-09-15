---
title: Profilsynkronisering
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: eee1080a95955332e205db3852381e39aaf5ae0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801763"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Hvornår ændres min profil til at blive synkroniseret med SharePoint-brugerprofilprogrammet?

SharePoint Online bruger Active Directory-import timerjobbet (AD-import) til at importere brugere og grupper til brugerprofilprogrammet. 
  
1. AD-import synkroniserer ændringer fra SharePoint Online-Biblioteks lageret til brugerprofilprogrammet. Disse ændringer behandles i batches.
    
2. Timerjobbet kører, indtil ændringerne er synkroniseret.
    
> [!NOTE]
> Den tid, det tager det job, der skal køres, afhænger af antallet af ændringer, der skal behandles. Et stort antal ændringer tager længere tid. Serviceniveauaftalen angiver, at en ændring af en bruger i SharePoint Online-kataloget vil blive afspejlet i brugerprofilprogrammet i 24 timer. 
  
[Flere oplysninger om synkronisering af brugerprofiler i SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

