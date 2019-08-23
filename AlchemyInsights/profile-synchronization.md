---
title: Synkronisering af brugerprofil
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36554327"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Når min profilændringer synkroniseres med SharePoint til brugerprofilprogrammet?

SharePoint Online bruger timerjobbet Active Directory-Import (Importer AD) til at importere brugere og grupper til brugerprofilprogrammet. 
  
1. AD Import synkroniserer ændringer fra SharePoint Online Directory Store brugerprofilprogrammet. Disse ændringer behandles i batches.
    
2. Timerjobbet kører, indtil ændringerne er synkroniserede.
    
> [!NOTE]
> Den tid, det tager at køre jobbet afhænger af antallet af ændringer til at behandle. Et stort antal ændringer tager længere tid. Service niveau aftale (SLA) angiver, at en ændring til en bruger i mappen SharePoint Online, afspejles i brugerprofilprogrammet inden for 24 timer. 
  
[Flere oplysninger om synkroniseringen af brugerprofilen i SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

