---
title: Fejlfinding i forbindelse med meddelelser, der er nægtet adgang
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 1930edcfd14acc48ea77b66e2793654a3e6332cc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759794"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="84ad8-102">Fejlfinding i forbindelse med meddelelser, der er nægtet adgang</span><span class="sxs-lookup"><span data-stu-id="84ad8-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="84ad8-103">Hvis nogen har fået meddelelsen "Adgang nægtet" til en delt mappe i SharePoint, har administratoren af gruppen af websteder muligvis aktiveret "Låsning af begrænset adgang til brugertilladelse".</span><span class="sxs-lookup"><span data-stu-id="84ad8-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="84ad8-104">Sådan slår du dette fra:</span><span class="sxs-lookup"><span data-stu-id="84ad8-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="84ad8-105">Gå til webstedet, klik på ikonet Indstillinger, og klik derefter på **Indstillinger for websted**.</span><span class="sxs-lookup"><span data-stu-id="84ad8-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="84ad8-106">Klik på Funktioner for **gruppe af websteder under**Administration af gruppe **af**websteder .</span><span class="sxs-lookup"><span data-stu-id="84ad8-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="84ad8-107">Klik på **Deaktiver**ud for **låsning af begrænset adgangstilladelse**.</span><span class="sxs-lookup"><span data-stu-id="84ad8-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="84ad8-108">Der kan også forekomme en meddelelse nægtet adgang for delte mapper, hvis webstedet er et publiceringswebsted.</span><span class="sxs-lookup"><span data-stu-id="84ad8-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="84ad8-109">Du kan finde oplysninger under [Access Denied, når du får adgang til en delt mappe](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="84ad8-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="84ad8-110">Hvis en person fik meddelelsen "Adgang nægtet", når vedkommende forsøger at få vist adgangsanmodninger, skal brugeren tilføjes som enten administrator af en gruppe af websteder eller medlem af gruppen Ejere for webstedet.</span><span class="sxs-lookup"><span data-stu-id="84ad8-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="84ad8-111">Du kan finde flere oplysninger på [listen Access Denied to Access Requests](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="84ad8-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="84ad8-112">Hvis en bruger fik meddelelsen "Adgang nægtet", efter at vedkommende blev fjernet fra Active Directory i det lokale miljø og derefter tilføjet igen, skal du se [Adgang nægtet, når en brugerkonto synkroniseres med Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="84ad8-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

