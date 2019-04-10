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
ms.openlocfilehash: 69e290e5a13f40ad045086791189a7d0af88240b
ms.sourcegitcommit: 228c986911ecf73217116a5d1fdcd2e89362774e
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/09/2019
ms.locfileid: "31747592"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="0e51d-102">Løse problemer med Deling af SharePoint-indhold med eksterne brugere</span><span class="sxs-lookup"><span data-stu-id="0e51d-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="0e51d-103">Sørg for, at eksterne deling er aktiveret for organisationen:</span><span class="sxs-lookup"><span data-stu-id="0e51d-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="0e51d-104">Gå til den [Services &amp; tilføjelsesprogrammer side i Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), og klik på **websteder**.</span><span class="sxs-lookup"><span data-stu-id="0e51d-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="0e51d-105">Kontroller, at indstillingen er slået til "On".</span><span class="sxs-lookup"><span data-stu-id="0e51d-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="0e51d-106">Hvis "Kun eksisterende eksterne brugere" er valgt, skal du kontrollere den eksterne bruger er angivet i Microsoft 365 admin center.</span><span class="sxs-lookup"><span data-stu-id="0e51d-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="0e51d-107">Kontroller, at Deling af den eksterne aktiveret for webstedet.</span><span class="sxs-lookup"><span data-stu-id="0e51d-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="0e51d-108">For en klassisk websteder:</span><span class="sxs-lookup"><span data-stu-id="0e51d-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="0e51d-109">Klik på **websteder**i det nye center på SharePoint-administrator i venstre rude.</span><span class="sxs-lookup"><span data-stu-id="0e51d-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="0e51d-110">Vælg den eller de websteder, og på båndet, skal du klikke på **Deling**.</span><span class="sxs-lookup"><span data-stu-id="0e51d-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="0e51d-111">For et websted for team, der tilhører en gruppe af Office 365, eller et kommunikationswebsted:</span><span class="sxs-lookup"><span data-stu-id="0e51d-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="0e51d-112">Disse nye websted har den samme deling indstilling som den globale indstilling, medmindre den globale indstilling tillader deling af filer ved hjælp af hyperlinks, der ikke kræver logon.</span><span class="sxs-lookup"><span data-stu-id="0e51d-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="0e51d-113">I dette tilfælde kan webstederne deler med nye og eksisterende eksterne brugere, der logger på.</span><span class="sxs-lookup"><span data-stu-id="0e51d-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="0e51d-114">Hvis du vil ændre indstillingen for bestemte websteder, ved at bruge nye SharePoint Administration center eller PowerShell.</span><span class="sxs-lookup"><span data-stu-id="0e51d-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="0e51d-115">[Få mere at vide](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="0e51d-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="0e51d-116">Indstillingen for eksterne deling for ethvert websted kan være mere restriktive end den globale indstilling, men ikke mere lempelige end den globale indstilling.</span><span class="sxs-lookup"><span data-stu-id="0e51d-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

