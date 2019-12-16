---
title: Arbejdsprocessen til godkendelse af 2010 kan ikke tilføjes
ms.author: pebaum
author: pebaum
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 11ba9bf04f826b0d7465a9a81a36c327e79f4d13
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049547"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="8f224-102">Arbejdsprocessen til godkendelse af 2010 kan ikke tilføjes</span><span class="sxs-lookup"><span data-stu-id="8f224-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="8f224-103">I en gruppe af Microsoft SharePoint-websteder kan du ikke føje en globalt genanvendelig arbejdsproces (f. eks. "godkendelse-SharePoint 2010") til en liste eller et bibliotek.</span><span class="sxs-lookup"><span data-stu-id="8f224-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="8f224-104">Du kan lÃ ̧se problemet ved at fÃ ̧lge disse trin:</span><span class="sxs-lookup"><span data-stu-id="8f224-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="8f224-105">Åbn rodwebstedet for gruppen af websteder i SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="8f224-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="8f224-106">Vælg **arbejdsprocesser**under **webstedsobjekter**.</span><span class="sxs-lookup"><span data-stu-id="8f224-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="8f224-107">I den **nye** sektion på båndet **arbejdsprocesser** skal du vælge **genanvendeligt workflow**.</span><span class="sxs-lookup"><span data-stu-id="8f224-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="8f224-108">Skriv navnet \* \* *Repair2010* \* \* i formularen **Opret genanvendeligt workflow** .</span><span class="sxs-lookup"><span data-stu-id="8f224-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="8f224-109">Klik på **SharePoint 2010-arbejdsproces**for **platforms type**, og klik derefter på **OK**.</span><span class="sxs-lookup"><span data-stu-id="8f224-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="8f224-110">I afsnittet **Gem** på båndet i **arbejdsgangen** skal du vælge **Udgiv**.</span><span class="sxs-lookup"><span data-stu-id="8f224-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="8f224-111">I afsnittet **Administrer** på båndet i **arbejdsgangen** skal du vælge **Udgiv globalt**.</span><span class="sxs-lookup"><span data-stu-id="8f224-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="8f224-112">I bekræftelsesdialogboksen, der vises, skal du vælge **OK**.</span><span class="sxs-lookup"><span data-stu-id="8f224-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="8f224-113">Find rodwebstedet for gruppen af websteder i en webbrowser, og Åbn \> derefter **funktionerne**for gruppen **af websteder.**</span><span class="sxs-lookup"><span data-stu-id="8f224-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="8f224-114">Slå funktionen **arbejdsprocesser** til:</span><span class="sxs-lookup"><span data-stu-id="8f224-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="8f224-115">· Hvis funktionen er *aktiveret* , skal du klikke på **Deaktiver** og derefter klikke på **Aktivér**.</span><span class="sxs-lookup"><span data-stu-id="8f224-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="8f224-116">· Klik på **Aktivér**, hvis funktionen er *deaktiveret* .</span><span class="sxs-lookup"><span data-stu-id="8f224-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="8f224-117">Yderligere oplysninger finder du i følgende [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="8f224-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

