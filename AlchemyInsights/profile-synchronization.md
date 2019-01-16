---
title: Synkronisering af brugerprofil
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: a32cf9e623d1be7a2c85ef4951c6eb7f001b7db0
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/15/2019
ms.locfileid: "28282823"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Når min profilændringer synkroniseres med SharePoint til brugerprofilprogrammet?

SharePoint Online bruger timerjobbet Active Directory-Import (Importer AD) til at importere brugere og grupper til brugerprofilprogrammet. 
  
1. AD Import synkroniserer ændringer fra SharePoint Online Directory Store brugerprofilprogrammet. Disse ændringer behandles i batches.
    
2. Timerjobbet kører, indtil ændringerne er synkroniserede.
    
> [!NOTE]
> Den tid, det tager at køre jobbet afhænger af antallet af ændringer til at behandle. Et stort antal ændringer tager længere tid. Service niveau aftale (SLA) angiver, at en ændring til en bruger i mappen SharePoint Online, afspejles i brugerprofilprogrammet inden for 24 timer. 
  
[Flere oplysninger om synkroniseringen af brugerprofilen i SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

