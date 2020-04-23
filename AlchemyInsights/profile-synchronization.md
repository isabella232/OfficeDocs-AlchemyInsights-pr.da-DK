---
title: Synkronisering af profiler
ms.author: arnek
author: arnek
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: dc6e0280961d14aa3e6bd466afbe0cbe89418d17
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43768107"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Hvornår synkroniseres mine profilændringer til SharePoint-brugerprofilprogrammet?

SharePoint Online bruger annonceimportjobbet (Active Directory Import Timer) til at importere brugere og grupper til brugerprofilprogrammet. 
  
1. AD Import synkroniserer ændringer fra SharePoint Online Directory Store til brugerprofilprogrammet. Disse ændringer behandles i batches.
    
2. Timerjobbet kører, indtil ændringerne synkroniseres.
    
> [!NOTE]
> Den tid, det tager jobbet at køre, afhænger af antallet af ændringer, der skal behandles. Et stort antal ændringer tager længere tid. SLA-aftalen (Service Level Agreement) angiver, at en ændring af en bruger i SharePoint Online Directory afspejles i brugerprofilprogrammet om 24 timer. 
  
[Flere oplysninger om synkronisering af brugerprofiler i SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

