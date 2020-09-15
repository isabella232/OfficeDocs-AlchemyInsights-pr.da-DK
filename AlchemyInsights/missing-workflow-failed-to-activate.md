---
title: Manglende arbejdsproces kunne ikke aktiveres
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 604dc770c5c14ded6a8de1cec9e311b03b69f094
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667080"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="5d345-102">Manglende arbejdsproces kunne ikke aktiveres</span><span class="sxs-lookup"><span data-stu-id="5d345-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="5d345-103">I en Microsoft SharePoint-gruppe af websteder kan du ikke tilføje en globalt genbrugelig arbejdsproces (f. eks "godkendelse-SharePoint 2010") på en liste eller i et bibliotek.</span><span class="sxs-lookup"><span data-stu-id="5d345-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="5d345-104">Du kan løse dette problem ved at følge disse trin:</span><span class="sxs-lookup"><span data-stu-id="5d345-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="5d345-105">Åbn rodwebstedet for gruppen af websteder i SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="5d345-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="5d345-106">Under **websteds objekter**skal du vælge **arbejdsprocesser**.</span><span class="sxs-lookup"><span data-stu-id="5d345-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="5d345-107">Vælg **arbejdsproces, der kan genbruges**, i den **nye** sektion på båndet **arbejdsprocesser** .</span><span class="sxs-lookup"><span data-stu-id="5d345-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="5d345-108">I formularen **Opret genbrugelig arbejdsproces** skal du angive navnet \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="5d345-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="5d345-109">For **platform type**skal du klikke på **SharePoint 2010-arbejdsproces**og derefter klikke på **OK**.</span><span class="sxs-lookup"><span data-stu-id="5d345-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="5d345-110">I sektionen **Gem** i båndet **arbejdsproces** skal du vælge **Publicer**.</span><span class="sxs-lookup"><span data-stu-id="5d345-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="5d345-111">I sektionen **Administrer** på båndet i **arbejdsproces** skal du vælge **Publicer globalt**.</span><span class="sxs-lookup"><span data-stu-id="5d345-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="5d345-112">I bekræftelsesdialogboksen, der vises, skal du vælge **OK**.</span><span class="sxs-lookup"><span data-stu-id="5d345-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="5d345-113">I en webbrowser skal du finde rodwebstedet for gruppen af websteder og derefter få adgang til funktioner **for gruppen** \> **af**websteder.</span><span class="sxs-lookup"><span data-stu-id="5d345-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="5d345-114">Derefter skal du slå **arbejdsproces** funktionen til/fra:</span><span class="sxs-lookup"><span data-stu-id="5d345-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="5d345-115">· Hvis funktionen er  *aktiveret*  , skal du **klikke på Deaktiver og** derefter klikke på **Aktivér**.</span><span class="sxs-lookup"><span data-stu-id="5d345-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="5d345-116">· Hvis funktionen er  *deaktiveret*  , skal du klikke på **Aktivér**.</span><span class="sxs-lookup"><span data-stu-id="5d345-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="5d345-117">Hvis du vil have mere at vide, skal du se følgende [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="5d345-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

