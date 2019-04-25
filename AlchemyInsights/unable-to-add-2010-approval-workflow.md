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
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/23/2019
ms.locfileid: "32366829"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="3a4ab-102">Kan ikke tilføjes 2010 godkendelsesforløb</span><span class="sxs-lookup"><span data-stu-id="3a4ab-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="3a4ab-103">I et Microsoft SharePoint-websteder, kan ikke du føje et globalt genbrugelig arbejdsproces (f.eks "godkendelse - SharePoint 2010") til en liste eller et bibliotek.</span><span class="sxs-lookup"><span data-stu-id="3a4ab-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="3a4ab-104">Du kan løse dette problem ved at følge disse trin:</span><span class="sxs-lookup"><span data-stu-id="3a4ab-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="3a4ab-105">Åbn rod-websted for gruppen af websteder i SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="3a4ab-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="3a4ab-106">Vælg **arbejdsprocesser**under **Objekter**.</span><span class="sxs-lookup"><span data-stu-id="3a4ab-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="3a4ab-107">Vælg **Arbejdsproces, kan genbruges**i afsnittet **Ny** i båndet **arbejdsprocesser** .</span><span class="sxs-lookup"><span data-stu-id="3a4ab-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="3a4ab-108">Angiv navnet formularen **Opret genanvendelig arbejdsproces** \*\* *Repair2010* \*\*.</span><span class="sxs-lookup"><span data-stu-id="3a4ab-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="3a4ab-109">Klik på **SharePoint 2010-arbejdsproces**til **Platform er af typen**, og klik derefter på **OK**.</span><span class="sxs-lookup"><span data-stu-id="3a4ab-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="3a4ab-110">Vælg **Udgiv**i afsnittet **Gem** i **arbejdsproces** -båndet.</span><span class="sxs-lookup"><span data-stu-id="3a4ab-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="3a4ab-111">Vælg **Udgiv globalt**i afsnittet **Manage** i **arbejdsproces** -båndet.</span><span class="sxs-lookup"><span data-stu-id="3a4ab-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="3a4ab-112">Klik på **OK**i bekræftelsesdialogboksen.</span><span class="sxs-lookup"><span data-stu-id="3a4ab-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="3a4ab-113">Find på rod-webstedet for gruppen af websteder i en webbrowser, og derefter få adgang til **Indstillinger for websted** \> **Funktioner på gruppen af websteder**.</span><span class="sxs-lookup"><span data-stu-id="3a4ab-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="3a4ab-114">Slå funktionen til **arbejdsprocesser** :</span><span class="sxs-lookup"><span data-stu-id="3a4ab-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="3a4ab-115">· Hvis funktionen er *aktiveret* , skal du klikke på **Deaktiver,** og klik derefter på **Aktiver**.</span><span class="sxs-lookup"><span data-stu-id="3a4ab-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="3a4ab-116">· Hvis funktionen er *deaktiveret* , skal du klikke på **Aktiver**.</span><span class="sxs-lookup"><span data-stu-id="3a4ab-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="3a4ab-117">Se følgende [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)for at få yderligere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="3a4ab-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

