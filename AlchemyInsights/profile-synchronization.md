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
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="68dd0-102">Hvornår ændres min profil til at blive synkroniseret med SharePoint-brugerprofilprogrammet?</span><span class="sxs-lookup"><span data-stu-id="68dd0-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="68dd0-103">SharePoint Online bruger Active Directory-import timerjobbet (AD-import) til at importere brugere og grupper til brugerprofilprogrammet.</span><span class="sxs-lookup"><span data-stu-id="68dd0-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="68dd0-104">AD-import synkroniserer ændringer fra SharePoint Online-Biblioteks lageret til brugerprofilprogrammet.</span><span class="sxs-lookup"><span data-stu-id="68dd0-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="68dd0-105">Disse ændringer behandles i batches.</span><span class="sxs-lookup"><span data-stu-id="68dd0-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="68dd0-106">Timerjobbet kører, indtil ændringerne er synkroniseret.</span><span class="sxs-lookup"><span data-stu-id="68dd0-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="68dd0-107">Den tid, det tager det job, der skal køres, afhænger af antallet af ændringer, der skal behandles.</span><span class="sxs-lookup"><span data-stu-id="68dd0-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="68dd0-108">Et stort antal ændringer tager længere tid.</span><span class="sxs-lookup"><span data-stu-id="68dd0-108">A large number of changes takes longer.</span></span> <span data-ttu-id="68dd0-109">Serviceniveauaftalen angiver, at en ændring af en bruger i SharePoint Online-kataloget vil blive afspejlet i brugerprofilprogrammet i 24 timer.</span><span class="sxs-lookup"><span data-stu-id="68dd0-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="68dd0-110">Flere oplysninger om synkronisering af brugerprofiler i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="68dd0-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

