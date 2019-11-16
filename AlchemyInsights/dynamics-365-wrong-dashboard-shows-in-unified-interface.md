---
title: Dynamics 365-forkerte Dashboard-programmer i Dynamics 365 Unified interface
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 11/15/2019
ms.locfileid: "36528545"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="e3dd4-102">Forkerte Dashboard-shows i Dynamics 365 Unified interface</span><span class="sxs-lookup"><span data-stu-id="e3dd4-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="e3dd4-103">Der er flere grunde til, at du kan se et andet dashboard end det, du forventer:</span><span class="sxs-lookup"><span data-stu-id="e3dd4-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="e3dd4-104">Brugeren har angivet et bruger standarddashboard</span><span class="sxs-lookup"><span data-stu-id="e3dd4-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="e3dd4-105">Typisk kan du identificere et bruger standarddashboard er indstillet, hvis knappen **Angiv som standard** ikke vises på Dashboard kommandolinjen.</span><span class="sxs-lookup"><span data-stu-id="e3dd4-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="e3dd4-106">Bruger standarddashboardet tilsidesætter alle andre standarddashboards, selvom brugerens standarddashboard ikke findes i den aktuelle app.</span><span class="sxs-lookup"><span data-stu-id="e3dd4-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="e3dd4-107">Brug følgende løsning til at fjerne et standarddashboard.</span><span class="sxs-lookup"><span data-stu-id="e3dd4-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="e3dd4-108">Opret et nyt personligt Dashboard.</span><span class="sxs-lookup"><span data-stu-id="e3dd4-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="e3dd4-109">Angiv det nye Dashboard som bruger standard.</span><span class="sxs-lookup"><span data-stu-id="e3dd4-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="e3dd4-110">Slet dashboardet.</span><span class="sxs-lookup"><span data-stu-id="e3dd4-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="e3dd4-111">Dashboardet er angivet i sitemap</span><span class="sxs-lookup"><span data-stu-id="e3dd4-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="e3dd4-112">Du har måske indstillet et organisations standarddashboard ved at vælge et dashboard og vælge ' Angiv som standard ' under ' Tilpas systemet '.</span><span class="sxs-lookup"><span data-stu-id="e3dd4-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="e3dd4-113">Men dashboardet, der er defineret i sitemap-designeren, har forrang for dette Dashboard, hvis brugeren har adgang til det.</span><span class="sxs-lookup"><span data-stu-id="e3dd4-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="e3dd4-114">Hvis brugerne skal kunne se det Dashboard, du har angivet som organisationens standard, kan du enten:</span><span class="sxs-lookup"><span data-stu-id="e3dd4-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="e3dd4-115">Indstil dashboardet i sitemap</span><span class="sxs-lookup"><span data-stu-id="e3dd4-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="e3dd4-116">Fjernadgang til det sitemap-definerede Dashboard for disse brugere</span><span class="sxs-lookup"><span data-stu-id="e3dd4-116">Remove access to the sitemap defined dashboard for those users</span></span>
