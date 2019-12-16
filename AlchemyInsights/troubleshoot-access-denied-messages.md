---
title: Fejlfinding i forbindelse med adgang nægtet-meddelelser
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 05d12aee49b449e8a29e84021b41298fb9983859
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050699"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="be91a-102">Fejlfinding i forbindelse med adgang nægtet-meddelelser</span><span class="sxs-lookup"><span data-stu-id="be91a-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="be91a-103">Hvis en person har fået meddelelsen "adgang nægtet" til en delt mappe i SharePoint, har administratoren af gruppen af websteder muligvis aktiveret "begrænset adgang til bruger tilladelses låsning".</span><span class="sxs-lookup"><span data-stu-id="be91a-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="be91a-104">Sådan deaktiverer du dette:</span><span class="sxs-lookup"><span data-stu-id="be91a-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="be91a-105">Gå til webstedet, klik på ikonet indstillinger, og klik derefter på **Indstillinger for websted**.</span><span class="sxs-lookup"><span data-stu-id="be91a-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="be91a-106">Klik på **funktioner for gruppen af**websteder under **administration af gruppe af**websteder.</span><span class="sxs-lookup"><span data-stu-id="be91a-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="be91a-107">Klik på **Deaktiver**ud for **tilstanden begrænset adgang til bruger tilladelse**.</span><span class="sxs-lookup"><span data-stu-id="be91a-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="be91a-108">Der kan også forekomme en meddelelse om adgang nægtet for delte mapper, hvis webstedet er et udgivelseswebsted.</span><span class="sxs-lookup"><span data-stu-id="be91a-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="be91a-109">Du kan finde flere oplysninger under [adgang nægtet, når du får adgang til en delt mappe](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="be91a-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="be91a-110">Hvis en person har fået meddelelsen "adgang nægtet", når du forsøger at få vist anmodninger om adgang, skal brugeren tilføjes enten som administrator af en gruppe af websteder eller som medlem af Ejergruppen for webstedet.</span><span class="sxs-lookup"><span data-stu-id="be91a-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="be91a-111">Du kan finde flere oplysninger under [adgang nægtet på listen over anmodninger om adgang](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="be91a-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="be91a-112">Hvis en bruger har fået meddelelsen "adgang nægtet", efter at de blev fjernet fra Active Directory i det lokale miljø og derefter tilføjet igen, [skal du se adgang nægtet, når en brugerkonto er synkroniseret med Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="be91a-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

