---
title: Arbejdsprocessen starter ikke
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 2d85dcf9111d48cb529c583c733823b404eb3188
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/25/2019
ms.locfileid: "36738083"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="76492-102">Arbejdsprocessen starter ikke</span><span class="sxs-lookup"><span data-stu-id="76492-102">Workflow is not starting</span></span>

- <span data-ttu-id="76492-103">Arbejdsprocesser i SharePoint 2010 og SharePoint 2013 starter ikke.</span><span class="sxs-lookup"><span data-stu-id="76492-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="76492-104">Hvis arbejdsprocessen ikke starter, kan der være et midlertidigt serviceproblem, hvor brugerne kan opleve periodiske forsinkelser med status for arbejdsprocessen.</span><span class="sxs-lookup"><span data-stu-id="76492-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="76492-105">Kontroller [dashboardet for tjenestetilstand](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) for at se, om din organisation påvirkes.</span><span class="sxs-lookup"><span data-stu-id="76492-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="76492-106">Hvis der er gået mere end 24 timer, siden du så dette problem, skal du logge en support billet.</span><span class="sxs-lookup"><span data-stu-id="76492-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="76492-107">I mange tilfælde arbejder vi allerede på en løsning.</span><span class="sxs-lookup"><span data-stu-id="76492-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="76492-108">Giv os mindst 24 timer til at gennemføre en løsning.</span><span class="sxs-lookup"><span data-stu-id="76492-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="76492-109">SharePoint 2010-arbejdsprocesser forsinket på Start.</span><span class="sxs-lookup"><span data-stu-id="76492-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="76492-110">Dette sker, hvis arbejdsprocessen udløses i store batches.</span><span class="sxs-lookup"><span data-stu-id="76492-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="76492-111">(f. eks. Når flere elementer tilføjes på én gang).</span><span class="sxs-lookup"><span data-stu-id="76492-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="76492-112">Arbejdsprocesser er ikke designet til at køre i realtid, så en forsinkelse er efter design-opførsel.</span><span class="sxs-lookup"><span data-stu-id="76492-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="76492-113">Hvis arbejdsprocessen er komplekst Extensible Object Markup Language (XMOL), kan kompileringen være langsom.</span><span class="sxs-lookup"><span data-stu-id="76492-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="76492-114">Tjek [denne](https://support.microsoft.com//kb/3043697) artikel.</span><span class="sxs-lookup"><span data-stu-id="76492-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="76492-115">Du bør forenkle arbejdsprocessen eller ændre den ved hjælp af Microsoft SharePoint 2013-arbejdsproces platforms typen.</span><span class="sxs-lookup"><span data-stu-id="76492-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="76492-116">Hvis din Arbejdsproceshistorik er blevet større, kan du slette emnerne eller oprette en ny oversigtsliste.</span><span class="sxs-lookup"><span data-stu-id="76492-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="76492-117">Flere oplysninger: [rydde Arbejdsproceshistorik](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="76492-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="76492-118">Relaterede emner</span><span class="sxs-lookup"><span data-stu-id="76492-118">Related topics</span></span>
<span data-ttu-id="76492-119">Vil du prøve Microsoft flow i SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="76492-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="76492-120">Opret flow</span><span class="sxs-lookup"><span data-stu-id="76492-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="76492-121">SharePoint og flow</span><span class="sxs-lookup"><span data-stu-id="76492-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


