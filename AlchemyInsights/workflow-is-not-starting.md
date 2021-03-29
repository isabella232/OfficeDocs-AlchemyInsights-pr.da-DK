---
title: Arbejdsprocessen er ikke startet
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403737"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="610cd-102">Arbejdsprocessen er ikke startet</span><span class="sxs-lookup"><span data-stu-id="610cd-102">Workflow is not starting</span></span>

- <span data-ttu-id="610cd-103">SharePoint 2010- og SharePoint 2013-arbejdsprocesser starter ikke.</span><span class="sxs-lookup"><span data-stu-id="610cd-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="610cd-104">Hvis arbejdsprocessen ikke starter, kan der være et midlertidigt tjenesteproblem, hvor brugere kan opleve forbigående forsinkelser med arbejdsprocesforløbet.</span><span class="sxs-lookup"><span data-stu-id="610cd-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="610cd-105">Kontrollér [dashboardet Tjenestetilstand for](https://admin.microsoft.com/AdminPortal/Home/servicehealth) at se, om din organisation påvirkes.</span><span class="sxs-lookup"><span data-stu-id="610cd-105">Check the [Service Health Dashboard](https://admin.microsoft.com/AdminPortal/Home/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="610cd-106">Hvis der er gået mere end 24 timer, siden du så dette problem første gang, skal du logge en supportanmodning.</span><span class="sxs-lookup"><span data-stu-id="610cd-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="610cd-107">I mange tilfælde arbejder vi allerede på en løsning.</span><span class="sxs-lookup"><span data-stu-id="610cd-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="610cd-108">Giv os mindst 24 timer til at fuldføre en løsning.</span><span class="sxs-lookup"><span data-stu-id="610cd-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="610cd-109">SharePoint 2010-arbejdsprocesser forsinket ved start.</span><span class="sxs-lookup"><span data-stu-id="610cd-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="610cd-110">Dette sker, hvis arbejdsprocessen udløses i store batches.</span><span class="sxs-lookup"><span data-stu-id="610cd-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="610cd-111">(f.eks. når flere elementer tilføjes på én gang).</span><span class="sxs-lookup"><span data-stu-id="610cd-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="610cd-112">Arbejdsprocesser er ikke designet til at køre i realtid, så en forsinkelse er en designfunktion.</span><span class="sxs-lookup"><span data-stu-id="610cd-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="610cd-113">Hvis arbejdsprocessen er kompleks Extensible Object Markup Language (XSUR), kan kompileringen være langsom.</span><span class="sxs-lookup"><span data-stu-id="610cd-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="610cd-114">Se [denne](https://support.microsoft.com//kb/3043697) artikel.</span><span class="sxs-lookup"><span data-stu-id="610cd-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="610cd-115">Du bør forenkle arbejdsprocessen eller omdesigne den ved hjælp af microsoft SharePoint 2013-arbejdsprocesplatformtypen.</span><span class="sxs-lookup"><span data-stu-id="610cd-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="610cd-116">Hvis arbejdsproceshistorikken er blevet stor, kan det være en god ide at fjerne elementerne eller oprette en ny oversigtsliste.</span><span class="sxs-lookup"><span data-stu-id="610cd-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="610cd-117">Flere oplysninger: [Slette arbejdsproceshistorik](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="610cd-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="610cd-118">Relaterede emner</span><span class="sxs-lookup"><span data-stu-id="610cd-118">Related topics</span></span>
<span data-ttu-id="610cd-119">Vil du prøve Microsoft Flow i SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="610cd-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="610cd-120">Opret flow</span><span class="sxs-lookup"><span data-stu-id="610cd-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="610cd-121">SharePoint og Flow</span><span class="sxs-lookup"><span data-stu-id="610cd-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
