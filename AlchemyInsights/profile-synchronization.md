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
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="eb15d-102">Hvornår synkroniseres min profil med SharePoint-brugerprofilprogrammet?</span><span class="sxs-lookup"><span data-stu-id="eb15d-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="eb15d-103">SharePoint Online bruger Active Directory-tids jobbet til import af timer (AD import) til at importere brugere og grupper til brugerprofilprogrammet.</span><span class="sxs-lookup"><span data-stu-id="eb15d-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="eb15d-104">AD import synkroniserer ændringer fra SharePoint Online-kataloglageret til brugerprofilprogrammet.</span><span class="sxs-lookup"><span data-stu-id="eb15d-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="eb15d-105">Disse ændringer behandles i batches.</span><span class="sxs-lookup"><span data-stu-id="eb15d-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="eb15d-106">Timerjobbet køres, indtil ændringerne er synkroniseret.</span><span class="sxs-lookup"><span data-stu-id="eb15d-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="eb15d-107">Den tid, det tager jobbet at køre, afhænger af antallet af ændringer, der skal udføres.</span><span class="sxs-lookup"><span data-stu-id="eb15d-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="eb15d-108">Et stort antal ændringer tager længere tid.</span><span class="sxs-lookup"><span data-stu-id="eb15d-108">A large number of changes takes longer.</span></span> <span data-ttu-id="eb15d-109">Serviceniveauaftalen (SLA) fastslår, at en ændring af en bruger i SharePoint Online-mappen vil blive afspejlet i brugerprofilprogrammet inden for 24 timer.</span><span class="sxs-lookup"><span data-stu-id="eb15d-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="eb15d-110">Flere oplysninger om Brugerprofilsynkronisering i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="eb15d-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

