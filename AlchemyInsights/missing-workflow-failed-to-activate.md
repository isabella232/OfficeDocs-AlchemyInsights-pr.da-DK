---
title: Den manglende arbejdsproces kunne ikke aktiveres
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 2598111005c219c398b63ca374e8e99348efc02c
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43762095"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="fc1ae-102">Den manglende arbejdsproces kunne ikke aktiveres</span><span class="sxs-lookup"><span data-stu-id="fc1ae-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="fc1ae-103">I en gruppe af Microsoft SharePoint-websteder kan du ikke føje en arbejdsproces, der kan genbruges globalt (f.eks.</span><span class="sxs-lookup"><span data-stu-id="fc1ae-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="fc1ae-104">Du kan lÃ ̧se problemet ved at fÃ ̧lge disse trin:</span><span class="sxs-lookup"><span data-stu-id="fc1ae-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="fc1ae-105">Åbn rodwebstedet for gruppen af websteder i SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="fc1ae-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="fc1ae-106">Vælg Arbejdsprocesser under **Webstedsobjekter**. **Workflows**</span><span class="sxs-lookup"><span data-stu-id="fc1ae-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="fc1ae-107">Vælg **Arbejdsproces, der kan** **genbruges,** i sektionen **Ny** på båndet Arbejdsprocesser .</span><span class="sxs-lookup"><span data-stu-id="fc1ae-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="fc1ae-108">Angiv navnet \*\* *Reparer2010* \*\*i formen **Opret genbrugelig arbejdsproces.**</span><span class="sxs-lookup"><span data-stu-id="fc1ae-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="fc1ae-109">Klik på **SharePoint 2010-arbejdsproces**for **Platformtype**, og klik derefter på **OK**.</span><span class="sxs-lookup"><span data-stu-id="fc1ae-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="fc1ae-110">Vælg **Publicer** i sektionen Gem på båndet **arbejdsproces** **.**</span><span class="sxs-lookup"><span data-stu-id="fc1ae-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="fc1ae-111">Vælg **Publicer** **globalt**i sektionen Administrer på båndet **arbejdsproces** .</span><span class="sxs-lookup"><span data-stu-id="fc1ae-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="fc1ae-112">Vælg **OK**i den bekræftelsesdialogboks, der vises .</span><span class="sxs-lookup"><span data-stu-id="fc1ae-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="fc1ae-113">Find rodwebstedet for gruppen af websteder i en webbrowser, og få derefter adgang til funktioner **til** \> **gruppe af websteder for websted**.</span><span class="sxs-lookup"><span data-stu-id="fc1ae-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="fc1ae-114">Slå derefter funktionen **Arbejdsprocesser** til/fra:</span><span class="sxs-lookup"><span data-stu-id="fc1ae-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="fc1ae-115">· Hvis funktionen er *Aktiveret* , skal du klikke på **Deaktiver** og derefter klikke på **Aktivér**.</span><span class="sxs-lookup"><span data-stu-id="fc1ae-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="fc1ae-116">· Hvis funktionen er *Deaktiveret* , skal du klikke på **Aktivér**.</span><span class="sxs-lookup"><span data-stu-id="fc1ae-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="fc1ae-117">Yderligere oplysninger finder du i følgende [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="fc1ae-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

