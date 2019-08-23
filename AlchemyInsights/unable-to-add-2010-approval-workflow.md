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
ms.openlocfilehash: 1f564c5d1e689dcf41b22fab5a05ab1b488c2b0b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36558611"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="84f50-102">Kan ikke tilføjes 2010 godkendelsesforløb</span><span class="sxs-lookup"><span data-stu-id="84f50-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="84f50-103">I et Microsoft SharePoint-websteder, kan ikke du føje et globalt genbrugelig arbejdsproces (f.eks "godkendelse - SharePoint 2010") til en liste eller et bibliotek.</span><span class="sxs-lookup"><span data-stu-id="84f50-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="84f50-104">Du kan løse dette problem ved at følge disse trin:</span><span class="sxs-lookup"><span data-stu-id="84f50-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="84f50-105">Åbn rod-websted for gruppen af websteder i SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="84f50-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="84f50-106">Vælg **arbejdsprocesser**under **Objekter**.</span><span class="sxs-lookup"><span data-stu-id="84f50-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="84f50-107">Vælg **Arbejdsproces, kan genbruges**i afsnittet **Ny** i båndet **arbejdsprocesser** .</span><span class="sxs-lookup"><span data-stu-id="84f50-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="84f50-108">Angiv navnet formularen **Opret genanvendelig arbejdsproces** \*\* *Repair2010* \*\*.</span><span class="sxs-lookup"><span data-stu-id="84f50-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="84f50-109">Klik på **SharePoint 2010-arbejdsproces**til **Platform er af typen**, og klik derefter på **OK**.</span><span class="sxs-lookup"><span data-stu-id="84f50-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="84f50-110">Vælg **Udgiv**i afsnittet **Gem** i **arbejdsproces** -båndet.</span><span class="sxs-lookup"><span data-stu-id="84f50-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="84f50-111">Vælg **Udgiv globalt**i afsnittet **Manage** i **arbejdsproces** -båndet.</span><span class="sxs-lookup"><span data-stu-id="84f50-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="84f50-112">Klik på **OK**i bekræftelsesdialogboksen.</span><span class="sxs-lookup"><span data-stu-id="84f50-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="84f50-113">Find på rod-webstedet for gruppen af websteder i en webbrowser, og derefter få adgang til **Indstillinger for websted** \> **Funktioner på gruppen af websteder**.</span><span class="sxs-lookup"><span data-stu-id="84f50-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="84f50-114">Slå funktionen til **arbejdsprocesser** :</span><span class="sxs-lookup"><span data-stu-id="84f50-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="84f50-115">· Hvis funktionen er *aktiveret* , skal du klikke på **Deaktiver,** og klik derefter på **Aktiver**.</span><span class="sxs-lookup"><span data-stu-id="84f50-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="84f50-116">· Hvis funktionen er *deaktiveret* , skal du klikke på **Aktiver**.</span><span class="sxs-lookup"><span data-stu-id="84f50-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="84f50-117">Se følgende [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)for at få yderligere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="84f50-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

