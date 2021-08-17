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
ms.openlocfilehash: a841db70c238bdae58edfca634fe49a04ddce78a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320703"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Hvornår synkroniseres mine profilændringer til SharePoint brugerprofilprogrammet?

SharePoint Online bruger Active Directory-import-timerjobbet (AD Import) til at importere brugere og grupper i brugerprofilprogrammet. 
  
1. AD-import synkroniserer ændringer fra SharePoint Online-Store til brugerprofilprogrammet. Disse ændringer behandles i batches.
    
2. Timerjobbet kører, indtil ændringerne synkroniseres.
    
**Bemærk!** Den tid, det tager at køre jobbet, afhænger af antallet af ændringer, der skal behandles. Et stort antal ændringer tager længere tid. Serviceaftaleaftalen (SERVICE Level Agreement) meddeler, at en ændring af en bruger i SharePoint Online Directory afspejles i brugerprofilprogrammet efter 24 timer. 
  
[Flere oplysninger om synkronisering af brugerprofiler i SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

