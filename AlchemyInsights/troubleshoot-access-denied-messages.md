---
title: Fejlfinding af adgang nægtet meddelelser
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 6c8ad84123fb58b73b9c378592ce970997893ea2
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704888"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="d6690-102">Fejlfinding af adgang nægtet meddelelser</span><span class="sxs-lookup"><span data-stu-id="d6690-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="d6690-103">Hvis nogen fik meddelelsen "Adgang nægtet" til en delt mappe i SharePoint, har administratoren af gruppen af websteder muligvis aktiveret "Låst tilstand for brugere med tilladelsen Begrænset adgang".</span><span class="sxs-lookup"><span data-stu-id="d6690-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="d6690-104">Sådan slår du dette fra:</span><span class="sxs-lookup"><span data-stu-id="d6690-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="d6690-105">Gå til webstedet, klik på ikonet Indstillinger, og klik derefter på **Indstillinger for websted.**</span><span class="sxs-lookup"><span data-stu-id="d6690-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="d6690-106">Klik **på Funktioner for grupper af** websteder under Administration af gruppe af **websteder.**</span><span class="sxs-lookup"><span data-stu-id="d6690-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="d6690-107">Ud for **låst tilstand for brugere med tilladelsen Begrænset adgang skal du** klikke på **Deaktiver.**</span><span class="sxs-lookup"><span data-stu-id="d6690-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="d6690-108">En Adgang nægtet-meddelelse kan også forekomme for delte mapper, hvis webstedet er et publiceringswebsted.</span><span class="sxs-lookup"><span data-stu-id="d6690-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="d6690-109">Du kan få mere at vide [under Adgang nægtet, når du åbner en delt mappe.](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb)</span><span class="sxs-lookup"><span data-stu-id="d6690-109">For info, see [Access Denied when accessing a shared folder](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span></span>
  
<span data-ttu-id="d6690-110">Hvis en person fik meddelelsen "Adgang nægtet", når han eller hun forsøger at få vist anmodninger om adgang, skal brugeren tilføjes som administrator for en gruppe af websteder eller som medlem af gruppen Ejere for webstedet.</span><span class="sxs-lookup"><span data-stu-id="d6690-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="d6690-111">Du kan finde flere oplysninger på [listen Anmodninger om adgang nægtet adgang.](https://go.microsoft.com/fwlink/?linkid=2004220)</span><span class="sxs-lookup"><span data-stu-id="d6690-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="d6690-112">Hvis en bruger fik meddelelsen "Adgang nægtet", efter brugeren blev fjernet fra Active Directory i det lokale miljø og derefter tilføjet igen, skal du se Adgang nægtet, når en brugerkonto synkroniseres med [Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=2004318)</span><span class="sxs-lookup"><span data-stu-id="d6690-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

