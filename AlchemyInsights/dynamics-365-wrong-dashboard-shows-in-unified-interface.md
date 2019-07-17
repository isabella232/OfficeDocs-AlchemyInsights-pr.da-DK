---
title: Dynamics 365 - forkert Dashboard viser i Dynamics 365 Unified grænseflade
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 6edf6fbae0174f3fa4d635c7a99e7daae1243b60
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/16/2019
ms.locfileid: "35747289"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="03793-102">Forkert dashboard viser i Dynamics 365 unified grænseflade</span><span class="sxs-lookup"><span data-stu-id="03793-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="03793-103">Der er flere grunde, hvorfor du kan se et andet dashboard end den, du forventer:</span><span class="sxs-lookup"><span data-stu-id="03793-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="03793-104">Brugeren har angivet et brugerdashboard standard</span><span class="sxs-lookup"><span data-stu-id="03793-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="03793-105">Typisk kan du identificere en bruger standarddashboard angives, hvis knappen **Vælg som standard** ikke vises på dashboard-kommandolinjen.</span><span class="sxs-lookup"><span data-stu-id="03793-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="03793-106">Standard brugerdashboard tilsidesætter alle andre standard dashboards, selvom brugerens standarddashboard ikke er i den aktuelle app.</span><span class="sxs-lookup"><span data-stu-id="03793-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="03793-107">Brug følgende fremgangsmåde til at fjerne deres standarddashboard.</span><span class="sxs-lookup"><span data-stu-id="03793-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="03793-108">Opret et nyt personligt instrumentbræt.</span><span class="sxs-lookup"><span data-stu-id="03793-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="03793-109">Angiv den nye dashboard som standard bruger.</span><span class="sxs-lookup"><span data-stu-id="03793-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="03793-110">Slet dette dashboard.</span><span class="sxs-lookup"><span data-stu-id="03793-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="03793-111">Dashboardet er angivet i sitemap</span><span class="sxs-lookup"><span data-stu-id="03793-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="03793-112">Du kan angive et standarddashboard for organisationen ved at vælge et dashboard og vælge 'Angiv som standard' under 'Tilpasse systemet'.</span><span class="sxs-lookup"><span data-stu-id="03793-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="03793-113">Men det dashboard, der er defineret i sitemap designer højere prioritet end dette dashboard, hvis brugeren har adgang til den.</span><span class="sxs-lookup"><span data-stu-id="03793-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="03793-114">Hvis brugerne kan se det dashboard, du har angivet som standard organisation, kan du enten:</span><span class="sxs-lookup"><span data-stu-id="03793-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="03793-115">Angiv dette dashboard i sitemap</span><span class="sxs-lookup"><span data-stu-id="03793-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="03793-116">Fjern adgang til dashboardet sitemap, der er defineret for disse brugere</span><span class="sxs-lookup"><span data-stu-id="03793-116">Remove access to the sitemap defined dashboard for those users</span></span>
