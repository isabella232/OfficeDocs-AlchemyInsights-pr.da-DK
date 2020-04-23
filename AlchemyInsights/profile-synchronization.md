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
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="991b8-102">Hvornår synkroniseres mine profilændringer til SharePoint-brugerprofilprogrammet?</span><span class="sxs-lookup"><span data-stu-id="991b8-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="991b8-103">SharePoint Online bruger annonceimportjobbet (Active Directory Import Timer) til at importere brugere og grupper til brugerprofilprogrammet.</span><span class="sxs-lookup"><span data-stu-id="991b8-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="991b8-104">AD Import synkroniserer ændringer fra SharePoint Online Directory Store til brugerprofilprogrammet.</span><span class="sxs-lookup"><span data-stu-id="991b8-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="991b8-105">Disse ændringer behandles i batches.</span><span class="sxs-lookup"><span data-stu-id="991b8-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="991b8-106">Timerjobbet kører, indtil ændringerne synkroniseres.</span><span class="sxs-lookup"><span data-stu-id="991b8-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="991b8-107">Den tid, det tager jobbet at køre, afhænger af antallet af ændringer, der skal behandles.</span><span class="sxs-lookup"><span data-stu-id="991b8-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="991b8-108">Et stort antal ændringer tager længere tid.</span><span class="sxs-lookup"><span data-stu-id="991b8-108">A large number of changes takes longer.</span></span> <span data-ttu-id="991b8-109">SLA-aftalen (Service Level Agreement) angiver, at en ændring af en bruger i SharePoint Online Directory afspejles i brugerprofilprogrammet om 24 timer.</span><span class="sxs-lookup"><span data-stu-id="991b8-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="991b8-110">Flere oplysninger om synkronisering af brugerprofiler i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="991b8-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

