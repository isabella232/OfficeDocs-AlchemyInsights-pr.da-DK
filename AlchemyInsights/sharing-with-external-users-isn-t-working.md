---
title: Deling med eksterne brugere fungerer ikke
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 285535d6144825f0935bf72579a483260c2f2bd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767243"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="51907-102">Løse problemer med at dele SharePoint-indhold med eksterne brugere</span><span class="sxs-lookup"><span data-stu-id="51907-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="51907-103">Sørg for, at ekstern deling er slået til for din organisation:</span><span class="sxs-lookup"><span data-stu-id="51907-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="51907-104">Gå til [ &amp; siden Med tilføjelsesprogrammet Tjenester i Microsoft 365 Administration](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), og klik på **Websteder**.</span><span class="sxs-lookup"><span data-stu-id="51907-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="51907-105">Sørg for, at indstillingen er slået til "Til".</span><span class="sxs-lookup"><span data-stu-id="51907-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="51907-106">Hvis "Kun eksisterende eksterne brugere" er valgt, skal du kontrollere, at den eksterne bruger er angivet i Microsoft 365 Administration.</span><span class="sxs-lookup"><span data-stu-id="51907-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="51907-107">Sørg for, at ekstern deling er slået til for webstedet.</span><span class="sxs-lookup"><span data-stu-id="51907-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="51907-108">For en klassisk gruppe af websteder:</span><span class="sxs-lookup"><span data-stu-id="51907-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="51907-109">Klik på **websteder**i venstre rude i den nye SharePoint Administration.</span><span class="sxs-lookup"><span data-stu-id="51907-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="51907-110">Vælg webstedet eller webstederne, og klik på **Deling**på båndet.</span><span class="sxs-lookup"><span data-stu-id="51907-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="51907-111">For et teamwebsted, der tilhører en Office 365-gruppe eller et kommunikationswebsted:</span><span class="sxs-lookup"><span data-stu-id="51907-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="51907-112">Disse nye webstedstyper har samme delingsindstilling som indstillingen for hele organisationen, medmindre indstillingen for hele organisationen tillader deling af filer ved hjælp af links, der ikke kræver logon.</span><span class="sxs-lookup"><span data-stu-id="51907-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="51907-113">I dette tilfælde tillader webstederne deling med nye og eksisterende eksterne brugere, der logger på.</span><span class="sxs-lookup"><span data-stu-id="51907-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="51907-114">Hvis du vil ændre indstillingen for bestemte websteder, skal du bruge det nye SharePoint Administration eller PowerShell.</span><span class="sxs-lookup"><span data-stu-id="51907-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="51907-115">[Få mere at vide](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="51907-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="51907-116">Indstillingen for ekstern deling for et hvilket som helst websted kan være mere restriktiv end indstillingen for hele organisationen, men ikke mere eftergivende end indstillingen for hele organisationen.</span><span class="sxs-lookup"><span data-stu-id="51907-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

