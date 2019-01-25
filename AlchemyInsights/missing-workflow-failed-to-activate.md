---
title: Manglende arbejdsprocessen kunne ikke aktiveres
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 33b92c2cae1f641b0cd88c82fd4ae5e8632d76c2
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/24/2019
ms.locfileid: "29463653"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="8ced9-102">Manglende arbejdsprocessen kunne ikke aktiveres</span><span class="sxs-lookup"><span data-stu-id="8ced9-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="8ced9-103">I et Microsoft SharePoint-websteder, kan ikke du føje et globalt genbrugelig arbejdsproces (f.eks "godkendelse - SharePoint 2010") til en liste eller et bibliotek.</span><span class="sxs-lookup"><span data-stu-id="8ced9-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="8ced9-104">Du kan løse dette problem ved at følge disse trin:</span><span class="sxs-lookup"><span data-stu-id="8ced9-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="8ced9-105">Åbn rod-websted for gruppen af websteder i SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="8ced9-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="8ced9-106">Vælg **arbejdsprocesser**under **Objekter**.</span><span class="sxs-lookup"><span data-stu-id="8ced9-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="8ced9-107">Vælg **Arbejdsproces, kan genbruges**i afsnittet **Ny** i båndet **arbejdsprocesser** .</span><span class="sxs-lookup"><span data-stu-id="8ced9-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="8ced9-p101">Angiv navnet formularen **Opret genanvendelig arbejdsproces** \*\* *Repair2010* \*\*. Klik på **SharePoint 2010-arbejdsproces**til **Platform er af typen**, og klik derefter på **OK**.</span><span class="sxs-lookup"><span data-stu-id="8ced9-p101">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*. For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="8ced9-110">Vælg **Udgiv**i afsnittet **Gem** i **arbejdsproces** -båndet.</span><span class="sxs-lookup"><span data-stu-id="8ced9-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="8ced9-p102">Vælg **Udgiv globalt**i afsnittet **Manage** i **arbejdsproces** -båndet. Klik på **OK**i bekræftelsesdialogboksen.</span><span class="sxs-lookup"><span data-stu-id="8ced9-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="8ced9-p103">Find på rod-webstedet for gruppen af websteder i en webbrowser, og derefter få adgang til **Indstillinger for websted** \> **Funktioner på gruppen af websteder**. Slå derefter funktionen **arbejdsprocesser** :</span><span class="sxs-lookup"><span data-stu-id="8ced9-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="8ced9-115">· Hvis funktionen er *aktiveret* , skal du klikke på **Deaktiver,** og klik derefter på **Aktiver**.</span><span class="sxs-lookup"><span data-stu-id="8ced9-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="8ced9-116">· Hvis funktionen er *deaktiveret* , skal du klikke på **Aktiver**.</span><span class="sxs-lookup"><span data-stu-id="8ced9-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="8ced9-117">Se følgende [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)for at få yderligere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="8ced9-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

