---
title: Kan ikke tilføjes 2010 godkendelsesforløb
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 3741b1169ddf731725c18fbaed80bfb321e5db46
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/12/2019
ms.locfileid: "29925410"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="43770-102">Kan ikke tilføjes 2010 godkendelsesforløb</span><span class="sxs-lookup"><span data-stu-id="43770-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="43770-103">I et Microsoft SharePoint-websteder, kan ikke du føje et globalt genbrugelig arbejdsproces (f.eks "godkendelse - SharePoint 2010") til en liste eller et bibliotek.</span><span class="sxs-lookup"><span data-stu-id="43770-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="43770-104">Du kan løse dette problem ved at følge disse trin:</span><span class="sxs-lookup"><span data-stu-id="43770-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="43770-105">Åbn rod-websted for gruppen af websteder i SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="43770-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="43770-106">Vælg **arbejdsprocesser**under **Objekter**.</span><span class="sxs-lookup"><span data-stu-id="43770-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="43770-107">Vælg **Arbejdsproces, kan genbruges**i afsnittet **Ny** i båndet **arbejdsprocesser** .</span><span class="sxs-lookup"><span data-stu-id="43770-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="43770-p101">Angiv navnet formularen **Opret genanvendelig arbejdsproces** \*\* *Repair2010* \*\*. Klik på **SharePoint 2010-arbejdsproces**til **Platform er af typen**, og klik derefter på **OK**.</span><span class="sxs-lookup"><span data-stu-id="43770-p101">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*. For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="43770-110">Vælg **Udgiv**i afsnittet **Gem** i **arbejdsproces** -båndet.</span><span class="sxs-lookup"><span data-stu-id="43770-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="43770-p102">Vælg **Udgiv globalt**i afsnittet **Manage** i **arbejdsproces** -båndet. Klik på **OK**i bekræftelsesdialogboksen.</span><span class="sxs-lookup"><span data-stu-id="43770-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="43770-p103">Find på rod-webstedet for gruppen af websteder i en webbrowser, og derefter få adgang til **Indstillinger for websted** \> **Funktioner på gruppen af websteder**. Slå funktionen til **arbejdsprocesser** :</span><span class="sxs-lookup"><span data-stu-id="43770-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="43770-115">· Hvis funktionen er *aktiveret* , skal du klikke på **Deaktiver,** og klik derefter på **Aktiver**.</span><span class="sxs-lookup"><span data-stu-id="43770-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="43770-116">· Hvis funktionen er *deaktiveret* , skal du klikke på **Aktiver**.</span><span class="sxs-lookup"><span data-stu-id="43770-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="43770-117">Se følgende [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)for at få yderligere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="43770-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

