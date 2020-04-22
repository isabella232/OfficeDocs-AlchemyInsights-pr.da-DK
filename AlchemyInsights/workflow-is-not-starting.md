---
title: Arbejdsprocessen starter ikke
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 941e6349c98278a1a8cdac77457ec1cc72cdef8b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766091"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="e8d82-102">Arbejdsprocessen starter ikke</span><span class="sxs-lookup"><span data-stu-id="e8d82-102">Workflow is not starting</span></span>

- <span data-ttu-id="e8d82-103">SharePoint 2010- og SharePoint 2013-arbejdsprocesser starter ikke.</span><span class="sxs-lookup"><span data-stu-id="e8d82-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="e8d82-104">Hvis arbejdsprocessen ikke starter, kan der være et midlertidigt tjenesteproblem, hvor brugerne kan opleve periodiske forsinkelser med arbejdsgangens fremdrift.</span><span class="sxs-lookup"><span data-stu-id="e8d82-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="e8d82-105">[Kontrollér Dashboardet for tjenestetilstand](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) for at se, om din organisation er påvirket.</span><span class="sxs-lookup"><span data-stu-id="e8d82-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="e8d82-106">Hvis der er gået mere end 24 timer, siden du første gang så dette problem, skal du logge en supportbillet.</span><span class="sxs-lookup"><span data-stu-id="e8d82-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="e8d82-107">I mange tilfælde arbejder vi allerede på en løsning.</span><span class="sxs-lookup"><span data-stu-id="e8d82-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="e8d82-108">Giv os mindst 24 timer til at fuldføre en løsning.</span><span class="sxs-lookup"><span data-stu-id="e8d82-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="e8d82-109">SharePoint 2010-arbejdsprocesser forsinket ved start.</span><span class="sxs-lookup"><span data-stu-id="e8d82-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="e8d82-110">Dette sker, hvis arbejdsprocessen udløses i store batches.</span><span class="sxs-lookup"><span data-stu-id="e8d82-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="e8d82-111">(f.eks. når der tilføjes flere elementer på én gang).</span><span class="sxs-lookup"><span data-stu-id="e8d82-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="e8d82-112">Arbejdsprocesser er ikke designet til at køre i realtid, så en forsinkelse er adfærd svære design.</span><span class="sxs-lookup"><span data-stu-id="e8d82-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="e8d82-113">Hvis arbejdsprocessen er kompleks XMOL (Extensible Object Markup Language), kan kompileringen være langsom.</span><span class="sxs-lookup"><span data-stu-id="e8d82-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="e8d82-114">Tjek [denne](https://support.microsoft.com//kb/3043697) artikel.</span><span class="sxs-lookup"><span data-stu-id="e8d82-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="e8d82-115">Du bør forenkle arbejdsprocessen eller ændre den ved hjælp af typen Af Typen af Microsoft SharePoint 2013 Workflow-platform.</span><span class="sxs-lookup"><span data-stu-id="e8d82-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="e8d82-116">Hvis arbejdsgangsoversigten er blevet stor, kan det være en god ide at fjerne elementerne eller oprette en ny oversigtsliste.</span><span class="sxs-lookup"><span data-stu-id="e8d82-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="e8d82-117">Flere oplysninger : [Fjern arbejdsproceshistorik](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="e8d82-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="e8d82-118">Relaterede emner</span><span class="sxs-lookup"><span data-stu-id="e8d82-118">Related topics</span></span>
<span data-ttu-id="e8d82-119">Vil du prøve Microsoft Flow i SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="e8d82-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="e8d82-120">Opret flow</span><span class="sxs-lookup"><span data-stu-id="e8d82-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="e8d82-121">SharePoint og Flow</span><span class="sxs-lookup"><span data-stu-id="e8d82-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


