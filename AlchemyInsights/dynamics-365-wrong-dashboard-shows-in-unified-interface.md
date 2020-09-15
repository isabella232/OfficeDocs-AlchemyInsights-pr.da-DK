---
title: Dynamics 365-forkert Dashboard vises i Dynamics 365 Unified interface
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711269"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="ca2a7-102">Forkert Dashboard vises i Dynamics 365 Unified interface</span><span class="sxs-lookup"><span data-stu-id="ca2a7-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="ca2a7-103">Der er flere årsager til, at du kan se et andet dashboard, end det, du forventer:</span><span class="sxs-lookup"><span data-stu-id="ca2a7-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="ca2a7-104">Brugeren har konfigureret et brugerdefineret Dashboard</span><span class="sxs-lookup"><span data-stu-id="ca2a7-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="ca2a7-105">Du kan typisk identificere et bruger standarddashboard, hvis knappen **Angiv som standard** ikke vises på Dashboard kommandolinjen.</span><span class="sxs-lookup"><span data-stu-id="ca2a7-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="ca2a7-106">Standard dashboardet for brugeren tilsidesætter alle andre standarddashboards, også selvom brugerens standarddashboard ikke er i den aktuelle app.</span><span class="sxs-lookup"><span data-stu-id="ca2a7-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="ca2a7-107">Brug følgende løsning til at fjerne standard dashboardet.</span><span class="sxs-lookup"><span data-stu-id="ca2a7-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="ca2a7-108">Opret et nyt personligt Dashboard.</span><span class="sxs-lookup"><span data-stu-id="ca2a7-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="ca2a7-109">Angiv det nye Dashboard som bruger standard.</span><span class="sxs-lookup"><span data-stu-id="ca2a7-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="ca2a7-110">Slet dette Dashboard.</span><span class="sxs-lookup"><span data-stu-id="ca2a7-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="ca2a7-111">Dashboardet er angivet i sitemap</span><span class="sxs-lookup"><span data-stu-id="ca2a7-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="ca2a7-112">Du har muligvis angivet et dashboard for organisationen ved at vælge et dashboard og vælge "Angiv som standard" under ' Tilpas systemet '.</span><span class="sxs-lookup"><span data-stu-id="ca2a7-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="ca2a7-113">Men det Dashboard, der er defineret i sitemap designer, tilsidesætter dette Dashboard, hvis brugeren har adgang til det.</span><span class="sxs-lookup"><span data-stu-id="ca2a7-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="ca2a7-114">Hvis du vil have brugerne til at se det Dashboard, du har angivet som organisations standard, kan du enten:</span><span class="sxs-lookup"><span data-stu-id="ca2a7-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="ca2a7-115">Indstille dette Dashboard i sitemap</span><span class="sxs-lookup"><span data-stu-id="ca2a7-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="ca2a7-116">Fjernadgang til det sitemap-Dashboard, der er defineret for disse brugere</span><span class="sxs-lookup"><span data-stu-id="ca2a7-116">Remove access to the sitemap defined dashboard for those users</span></span>
