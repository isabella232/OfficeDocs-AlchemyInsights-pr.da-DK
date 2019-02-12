---
title: Fejlfinding i forbindelse med meddelelser adgang nægtet
ms.author: kaarins
author: kaarins
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: f1a4803838b6511ef4fe7f03cafa4aa13b3c9734
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/12/2019
ms.locfileid: "29916446"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="153ae-102">Fejlfinding i forbindelse med meddelelser adgang nægtet</span><span class="sxs-lookup"><span data-stu-id="153ae-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="153ae-p101">Hvis en person har fået en "Adgang nægtet"-meddelelse til en delt mappe, kan administratoren af gruppen af websteder har aktiveret "begrænset adgang tilladelse lockdown brugertilstand." Du kan slå denne indstilling fra:</span><span class="sxs-lookup"><span data-stu-id="153ae-p101">If someone got an "Access Denied" message to a shared folder, the site collection administrator might have enabled "Limited-access user permission lockdown mode." To turn this off:</span></span> 
  
1. <span data-ttu-id="153ae-105">Gå til webstedet, skal du klikke på ikonet indstillinger, og klik derefter på **Indstillinger for websted**.</span><span class="sxs-lookup"><span data-stu-id="153ae-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="153ae-106">Klik på **funktioner på gruppen af websteder**under **Administration af gruppe af websteder**.</span><span class="sxs-lookup"><span data-stu-id="153ae-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="153ae-107">Klik på **Deaktiver**ud for **begrænset adgang tilladelse lockdown brugertilstand**.</span><span class="sxs-lookup"><span data-stu-id="153ae-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="153ae-p102">Meddelelsen adgang nægtet kan også opstå for delte mapper, hvis webstedet er et udgivelseswebsted. Oplysninger, finder du i [Adgang nægtet, når du åbner en delt mappe](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="153ae-p102">An Access Denied message can also occur for shared folders if the site is a publishing site. For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="153ae-p103">Hvis en anden har modtaget meddelelsen "Adgang nægtet", når du forsøger at få vist anmodninger om adgang, skal som brugeren tilføjes som en webstedsadministrator eller medlem af gruppen Ejere på webstedet. Yderligere oplysninger finder du i [Adgang til listen over anmodninger om adgang nægtet](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="153ae-p103">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site. For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="153ae-112">Hvis en bruger har fået meddelelsen "Adgang nægtet", når de er fjernet fra Active Directory på stedet og derefter tilføjes igen, kan du se [Adgang nægtet, når en brugerkonto, der er synkroniseret med Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="153ae-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

