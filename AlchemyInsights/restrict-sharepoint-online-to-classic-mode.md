---
title: Begræns SharePoint Online til klassisk tilstand
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: c5ea5d264b62e4c349623bd431776207b38da470
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742463"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="c92bd-102">Begræns SharePoint Online til klassisk tilstand</span><span class="sxs-lookup"><span data-stu-id="c92bd-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="c92bd-103">Nogle organisationer kræver stadig den klassiske tilstandsoplevelse.</span><span class="sxs-lookup"><span data-stu-id="c92bd-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="c92bd-104">Selvom der ikke er planer om at fjerne klassisk tilstand på et detaljeret niveau, er det ikke længere muligt at begrænse en hel organisation (lejer) til klassisk tilstand for lister og biblioteker.</span><span class="sxs-lookup"><span data-stu-id="c92bd-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="c92bd-105">Administratoren har følgende muligheder for at administrere individuelle lister og biblioteker i klassisk tilstand ved hjælp af detaljerede fravalgsparametre, som vi leverer på følgende niveauer:</span><span class="sxs-lookup"><span data-stu-id="c92bd-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="c92bd-106">gruppe af websteder</span><span class="sxs-lookup"><span data-stu-id="c92bd-106">site collection</span></span>
- <span data-ttu-id="c92bd-107">Websted</span><span class="sxs-lookup"><span data-stu-id="c92bd-107">site</span></span>
- <span data-ttu-id="c92bd-108">Liste</span><span class="sxs-lookup"><span data-stu-id="c92bd-108">list</span></span>
- <span data-ttu-id="c92bd-109">Bibliotek</span><span class="sxs-lookup"><span data-stu-id="c92bd-109">library</span></span>

<span data-ttu-id="c92bd-110">Derudover vil lister, der bruger bestemte funktioner og tilpasninger, der ikke understøttes af moderne, stadig automatisk blive skiftet til klassisk tilstand.</span><span class="sxs-lookup"><span data-stu-id="c92bd-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="c92bd-111">april 2019 starter processen med at deaktivere lejerniveaufravalg af moderne liste og biblioteker frem til 31. maj 2019.</span><span class="sxs-lookup"><span data-stu-id="c92bd-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="c92bd-112">De lister og biblioteker, der er i klassisk tilstand som følge af lejer opt-out, vil automatisk blive flyttet til moderne.</span><span class="sxs-lookup"><span data-stu-id="c92bd-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="c92bd-113">Hvis du har brug for klassisk tilstand kan du se mere information [her](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) og PnP Powershell instruktion [her,](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) der beskriver muligheder og værktøjer, du kan bruge i dag til at bruge den klassiske tilstand oplevelse.</span><span class="sxs-lookup"><span data-stu-id="c92bd-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
