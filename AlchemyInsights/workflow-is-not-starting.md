---
title: Arbejdsprocessen starter ikke
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
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794761"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="cf197-102">Arbejdsprocessen starter ikke</span><span class="sxs-lookup"><span data-stu-id="cf197-102">Workflow is not starting</span></span>

- <span data-ttu-id="cf197-103">SharePoint 2010-og SharePoint 2013-arbejdsprocesser starter ikke.</span><span class="sxs-lookup"><span data-stu-id="cf197-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="cf197-104">Hvis arbejdsprocessen ikke starter, kan der være et midlertidigt tjeneste problem, hvor brugerne kan opleve periodiske forsinkelser med arbejdsprocesstatus.</span><span class="sxs-lookup"><span data-stu-id="cf197-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="cf197-105">Se [dashboardet for tjenestetilstand](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) for at se, om din organisation er påvirket.</span><span class="sxs-lookup"><span data-stu-id="cf197-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="cf197-106">Hvis der er gået mere end 24 timer, siden du først fik dette problem, skal du logge på en support billet.</span><span class="sxs-lookup"><span data-stu-id="cf197-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="cf197-107">I mange tilfælde arbejder vi allerede på en løsning.</span><span class="sxs-lookup"><span data-stu-id="cf197-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="cf197-108">Giv os mindst 24 timer for at fuldføre en løsning.</span><span class="sxs-lookup"><span data-stu-id="cf197-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="cf197-109">SharePoint 2010-arbejdsprocesser forsinkede start.</span><span class="sxs-lookup"><span data-stu-id="cf197-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="cf197-110">Dette sker, hvis arbejdsprocessen udløses i store batches.</span><span class="sxs-lookup"><span data-stu-id="cf197-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="cf197-111">(f. eks. Når flere elementer tilføjes på én gang).</span><span class="sxs-lookup"><span data-stu-id="cf197-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="cf197-112">Arbejdsprocesser er ikke beregnet til at køre realtid, så en forsinkelse er en funktionsmåde.</span><span class="sxs-lookup"><span data-stu-id="cf197-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="cf197-113">Hvis arbejdsprocessen er komplekst XMOL (Extensible Object Markup Language), kan kompileringen være langsom.</span><span class="sxs-lookup"><span data-stu-id="cf197-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="cf197-114">Se [denne](https://support.microsoft.com//kb/3043697) artikel.</span><span class="sxs-lookup"><span data-stu-id="cf197-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="cf197-115">Du bør forenkle arbejdsprocessen eller ændre designet ved hjælp af Microsoft SharePoint 2013 workflow platform-typen.</span><span class="sxs-lookup"><span data-stu-id="cf197-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="cf197-116">Hvis din Arbejdsproceshistorik er blevet stor, kan det være en god ide at slette elementerne eller oprette en ny oversigtsliste.</span><span class="sxs-lookup"><span data-stu-id="cf197-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="cf197-117">Flere oplysninger: [rydde oversigt over arbejdsprocesser](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="cf197-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="cf197-118">Relaterede emner</span><span class="sxs-lookup"><span data-stu-id="cf197-118">Related topics</span></span>
<span data-ttu-id="cf197-119">Vil du prøve Microsoft flow i SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="cf197-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="cf197-120">Opret flow</span><span class="sxs-lookup"><span data-stu-id="cf197-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="cf197-121">SharePoint og flow</span><span class="sxs-lookup"><span data-stu-id="cf197-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


