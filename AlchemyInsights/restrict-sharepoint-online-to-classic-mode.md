---
title: Begrænse SharePoint Online til klassisk tilstand
ms.author: pebaum
author: Techwriter40
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 18d263593d99f24c3020336ae601df14dbbf5411
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/18/2019
ms.locfileid: "36752062"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="744ca-102">Begrænse SharePoint Online til klassisk tilstand</span><span class="sxs-lookup"><span data-stu-id="744ca-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="744ca-103">Nogle organisationer kræver stadig den klassiske tilstands oplevelse.</span><span class="sxs-lookup"><span data-stu-id="744ca-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="744ca-104">Selvom der ikke er planer om at fjerne klassisk tilstand på et detaljeret niveau, er det ikke længere muligt at begrænse en hel organisation (lejer) til klassisk tilstand for lister og biblioteker.</span><span class="sxs-lookup"><span data-stu-id="744ca-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="744ca-105">Administratoren vil have følgende muligheder for at administrere individuelle lister og biblioteker i klassisk tilstand ved hjælp af granulære fravalgs parametre, som vi leverer på følgende niveauer:</span><span class="sxs-lookup"><span data-stu-id="744ca-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="744ca-106">gruppe af websteder</span><span class="sxs-lookup"><span data-stu-id="744ca-106">site collection</span></span>
- <span data-ttu-id="744ca-107">Websted</span><span class="sxs-lookup"><span data-stu-id="744ca-107">site</span></span>
- <span data-ttu-id="744ca-108">Liste</span><span class="sxs-lookup"><span data-stu-id="744ca-108">list</span></span>
- <span data-ttu-id="744ca-109">Bibliotek</span><span class="sxs-lookup"><span data-stu-id="744ca-109">library</span></span>

<span data-ttu-id="744ca-110">Desuden vil lister, der bruger visse funktioner og tilpasninger, som ikke understøttes af Modern, stadig automatisk blive skiftet til klassisk tilstand.</span><span class="sxs-lookup"><span data-stu-id="744ca-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="744ca-111">Begyndende april 1, 2019, den oparbejde hen til forhindre den lejer plan opt op fra moderne liste og biblioteker vil opståen og fortsætte igennem må 31, 2019.</span><span class="sxs-lookup"><span data-stu-id="744ca-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="744ca-112">De lister og biblioteker, der er i klassisk tilstand som et resultat af lejer fravalg, vil automatisk blive flyttet til Modern.</span><span class="sxs-lookup"><span data-stu-id="744ca-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="744ca-113">Hvis du har brug for klassisk tilstand, skal du se flere oplysninger [her](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) og PnP PowerShell instruktion [her](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) , der beskriver muligheder og værktøjer, du kan bruge i dag til at bruge den klassiske tilstand oplevelse.</span><span class="sxs-lookup"><span data-stu-id="744ca-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
