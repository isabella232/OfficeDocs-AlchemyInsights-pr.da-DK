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
ms.openlocfilehash: d4bfdb44c04eb6838f4a265e55a4873d14c78f6d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36557963"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="8e6d8-102">Arbejdsprocessen starter ikke</span><span class="sxs-lookup"><span data-stu-id="8e6d8-102">Workflow is not starting</span></span>

- <span data-ttu-id="8e6d8-103">Arbejdsgange i SharePoint 2010, og SharePoint 2013 starter ikke.</span><span class="sxs-lookup"><span data-stu-id="8e6d8-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="8e6d8-104">Hvis arbejdsprocessen ikke starter, kan der være et problem med den midlertidige tjeneste hvor brugere kan opleve forbigående forsinkelser med status for arbejdsprocessen.</span><span class="sxs-lookup"><span data-stu-id="8e6d8-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="8e6d8-105">Kontroller [Service sundhed Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) for at se, hvis organisationen påvirkes.</span><span class="sxs-lookup"><span data-stu-id="8e6d8-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="8e6d8-106">Hvis der er gået mere end 24 timer, da du så først problemet, skal du logge en støtte billet.</span><span class="sxs-lookup"><span data-stu-id="8e6d8-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="8e6d8-107">I mange tilfælde kan arbejder vi allerede på en løsning.</span><span class="sxs-lookup"><span data-stu-id="8e6d8-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="8e6d8-108">Giv os, mindst 24 timer at gennemføre en løsning.</span><span class="sxs-lookup"><span data-stu-id="8e6d8-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="8e6d8-109">SharePoint 2010-arbejdsprocesser forsinkelse ved start.</span><span class="sxs-lookup"><span data-stu-id="8e6d8-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="8e6d8-110">Dette sker, hvis arbejdsprocessen udløses i store partier.</span><span class="sxs-lookup"><span data-stu-id="8e6d8-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="8e6d8-111">(for eksempel, når flere elementer tilføjes på én gang).</span><span class="sxs-lookup"><span data-stu-id="8e6d8-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="8e6d8-112">Arbejdsprocesser er ikke beregnet til at køre i realtid, så en forsinkelse er tilsigtet funktionsmåde.</span><span class="sxs-lookup"><span data-stu-id="8e6d8-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="8e6d8-113">Kompileringen kan være langsom, hvis arbejdsgangen er komplekse Extensible objekt Markup Language (XMOL).</span><span class="sxs-lookup"><span data-stu-id="8e6d8-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="8e6d8-114">Læs [denne](https://support.microsoft.com/en-us/kb/3043697) artikel.</span><span class="sxs-lookup"><span data-stu-id="8e6d8-114">Check [this](https://support.microsoft.com/en-us/kb/3043697) article.</span></span>

    - <span data-ttu-id="8e6d8-115">Du bør forenkle arbejdsgangen eller designe det ved hjælp af Microsoft SharePoint 2013 platform arbejdsgangstype.</span><span class="sxs-lookup"><span data-stu-id="8e6d8-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="8e6d8-116">Hvis din arbejdsgangshistorikken er blevet stort, kan du fjerne varerne eller oprette en ny oversigtsliste.</span><span class="sxs-lookup"><span data-stu-id="8e6d8-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="8e6d8-117">Yderligere oplysninger: [Fjern arbejdsgangshistorik](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="8e6d8-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="8e6d8-118">Relaterede emner</span><span class="sxs-lookup"><span data-stu-id="8e6d8-118">Related topics</span></span>
<span data-ttu-id="8e6d8-119">Vil du prøve Microsoft Flow i SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="8e6d8-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="8e6d8-120">Oprette produktionsflow</span><span class="sxs-lookup"><span data-stu-id="8e6d8-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="8e6d8-121">SharePoint og Flow</span><span class="sxs-lookup"><span data-stu-id="8e6d8-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


