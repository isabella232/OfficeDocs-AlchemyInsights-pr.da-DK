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
ms.openlocfilehash: b223bad66fb7cc6d1d7c0a2b3ccc7a081c061b4974060dbcafec84dfb24eb782
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923638"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Hvornår synkroniseres min profil med SharePoint brugerprofilprogrammet?

SharePoint Online bruger Active Directory-import-timerjobbet (AD Import) til at importere brugere og grupper i brugerprofilprogrammet. 
  
1. AD-import synkroniserer ændringer fra SharePoint Online Directory Store til brugerprofilprogrammet. Disse ændringer behandles i batches.
    
2. Timerjobbet kører, indtil ændringerne synkroniseres.
    
> [!NOTE]
> Den tid, det tager at køre jobbet, afhænger af antallet af ændringer, der skal behandles. Et stort antal ændringer tager længere tid. Serviceaftaleaftalen (SLA) meddeler, at en ændring af en bruger i SharePoint Online Directory afspejles i brugerprofilprogrammet efter 24 timer. 
  
[Flere oplysninger om synkronisering af brugerprofiler i SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

