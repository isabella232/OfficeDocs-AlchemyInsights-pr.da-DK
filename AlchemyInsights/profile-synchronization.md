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
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/24/2019
ms.locfileid: "29464522"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="8ac36-102">Når min profilændringer synkroniseres med SharePoint til brugerprofilprogrammet?</span><span class="sxs-lookup"><span data-stu-id="8ac36-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="8ac36-103">SharePoint Online bruger timerjobbet Active Directory-Import (Importer AD) til at importere brugere og grupper til brugerprofilprogrammet.</span><span class="sxs-lookup"><span data-stu-id="8ac36-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="8ac36-p101">AD Import synkroniserer ændringer fra SharePoint Online Directory Store brugerprofilprogrammet. Disse ændringer behandles i batches.</span><span class="sxs-lookup"><span data-stu-id="8ac36-p101">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application. These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="8ac36-106">Timerjobbet kører, indtil ændringerne er synkroniserede.</span><span class="sxs-lookup"><span data-stu-id="8ac36-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="8ac36-p102">Den tid, det tager at køre jobbet afhænger af antallet af ændringer til at behandle. Et stort antal ændringer tager længere tid. Service niveau aftale (SLA) angiver, at en ændring til en bruger i mappen SharePoint Online, afspejles i brugerprofilprogrammet inden for 24 timer.</span><span class="sxs-lookup"><span data-stu-id="8ac36-p102">The time it takes the job to run depends on the number of changes to process. A large number of changes takes longer. The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="8ac36-110">Flere oplysninger om synkroniseringen af brugerprofilen i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="8ac36-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

