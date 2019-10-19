---
title: Deling med eksterne brugere fungerer ikke
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: d4c8fc75ff8db2319b88a20bea9b3ee661f2e36e
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/18/2019
ms.locfileid: "36502225"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="f801f-102">Løs problemer med deling af SharePoint-indhold med eksterne brugere</span><span class="sxs-lookup"><span data-stu-id="f801f-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="f801f-103">Sørg for, at ekstern deling er slået til for din organisation:</span><span class="sxs-lookup"><span data-stu-id="f801f-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="f801f-104">Gå til [siden med &amp; tilføjelsesprogrammer til tjenester i Microsoft 365 administration](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), og klik på **websteder**.</span><span class="sxs-lookup"><span data-stu-id="f801f-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="f801f-105">Sørg for, at indstillingen er slået til "til".</span><span class="sxs-lookup"><span data-stu-id="f801f-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="f801f-106">Hvis "kun eksisterende eksterne brugere" er valgt, skal du kontrollere, at den eksterne bruger er angivet i Microsoft 365 administration.</span><span class="sxs-lookup"><span data-stu-id="f801f-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="f801f-107">Sørg for, at ekstern deling det er slået til for webstedet.</span><span class="sxs-lookup"><span data-stu-id="f801f-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="f801f-108">For en klassisk gruppe af websteder:</span><span class="sxs-lookup"><span data-stu-id="f801f-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="f801f-109">Klik på **websteder**i den venstre rude i det nye SharePoint-Administrationscenter.</span><span class="sxs-lookup"><span data-stu-id="f801f-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="f801f-110">Vælg webstedet eller webstederne, og klik på **deling**på båndet.</span><span class="sxs-lookup"><span data-stu-id="f801f-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="f801f-111">For et teamwebsted, der tilhører en Office 365-gruppe, eller et kommunikationswebsted:</span><span class="sxs-lookup"><span data-stu-id="f801f-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="f801f-112">Disse nye webstedstyper har samme delingsindstilling som indstillingen for hele organisationen, medmindre indstillingen for hele organisationen tillader deling af filer ved hjælp af links, der ikke kræver logon.</span><span class="sxs-lookup"><span data-stu-id="f801f-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="f801f-113">I dette tilfælde tillader webstederne deling med nye og eksisterende eksterne brugere, der logger på.</span><span class="sxs-lookup"><span data-stu-id="f801f-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="f801f-114">Hvis du vil ændre indstillingen for bestemte websteder, skal du bruge det nye SharePoint-Administrationscenter eller PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f801f-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="f801f-115">[Læs mere](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="f801f-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="f801f-116">Den eksterne delingsindstilling for et hvilket som helst websted kan være mere restriktiv end organisationens indstillinger, men ikke mere eftergivende end den globale indstilling.</span><span class="sxs-lookup"><span data-stu-id="f801f-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

