---
title: Foretag fejlfinding af meddelelser om nægtet adgang
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3550081a12379f73725253214a2c2d44974ab740
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690777"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="fee9b-102">Foretag fejlfinding af meddelelser om nægtet adgang</span><span class="sxs-lookup"><span data-stu-id="fee9b-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="fee9b-103">Hvis en person har fået meddelelsen "adgang nægtet" til en delt mappe i SharePoint, kan administratoren af gruppen af websteder have aktiveret tilstanden begrænset adgang til bruger rettigheds låsning.</span><span class="sxs-lookup"><span data-stu-id="fee9b-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="fee9b-104">Sådan deaktiveres:</span><span class="sxs-lookup"><span data-stu-id="fee9b-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="fee9b-105">Gå til webstedet, klik på ikonet indstillinger, og klik derefter på **Indstillinger for websted**.</span><span class="sxs-lookup"><span data-stu-id="fee9b-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="fee9b-106">Klik på **funktioner for gruppen af**websteder under **administration af gruppe af websteder**.</span><span class="sxs-lookup"><span data-stu-id="fee9b-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="fee9b-107">Klik på **Deaktiver**ud for **tilstanden begrænset adgang til bruger rettigheds låsning**.</span><span class="sxs-lookup"><span data-stu-id="fee9b-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="fee9b-108">En meddelelse om adgang nægtet kan også forekomme for delte mapper, hvis webstedet er et publiceringswebsted.</span><span class="sxs-lookup"><span data-stu-id="fee9b-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="fee9b-109">Hvis du vil have mere at vide, skal du se [adgang nægtet, når du åbner en delt mappe](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="fee9b-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="fee9b-110">Hvis en person har fået meddelelsen "adgang nægtet", når du forsøger at få vist adgangsanmodninger, skal brugeren enten tilføjes som administrator af en gruppe af websteder eller medlem af gruppen ejere for webstedet.</span><span class="sxs-lookup"><span data-stu-id="fee9b-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="fee9b-111">Hvis du vil have mere at vide, skal du se [adgang nægtet til listen over anmodninger om adgang](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="fee9b-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="fee9b-112">Hvis en bruger har fået meddelelsen "adgang nægtet", efter at vedkommende er blevet fjernet fra Active Directory i det lokale miljø og derefter tilføjet tilbage, skal du se [adgang nægtet, når en brugerkonto synkroniseres med Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="fee9b-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

