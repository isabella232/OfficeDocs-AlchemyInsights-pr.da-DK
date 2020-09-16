---
title: Begræns SharePoint Online til klassisk tilstand
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751416"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="2d2e6-102">Begræns SharePoint Online til klassisk tilstand</span><span class="sxs-lookup"><span data-stu-id="2d2e6-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="2d2e6-103">Nogle organisationer kræver stadig den klassiske oplevelse af tilstanden.</span><span class="sxs-lookup"><span data-stu-id="2d2e6-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="2d2e6-104">Selvom der ikke er nogen planer om at fjerne klassisk tilstand på et detaljeret niveau, er det ikke længere muligt at begrænse en hel organisation (lejer) til klassisk tilstand for lister og biblioteker.</span><span class="sxs-lookup"><span data-stu-id="2d2e6-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="2d2e6-105">Administratoren har følgende muligheder for at administrere individuelle lister og biblioteker i klassisk tilstand med detaljerede afleverings parametre, som vi giver på følgende niveauer:</span><span class="sxs-lookup"><span data-stu-id="2d2e6-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="2d2e6-106">gruppe af websteder</span><span class="sxs-lookup"><span data-stu-id="2d2e6-106">site collection</span></span>
- <span data-ttu-id="2d2e6-107">adresse</span><span class="sxs-lookup"><span data-stu-id="2d2e6-107">site</span></span>
- <span data-ttu-id="2d2e6-108">liste</span><span class="sxs-lookup"><span data-stu-id="2d2e6-108">list</span></span>
- <span data-ttu-id="2d2e6-109">bibliotek</span><span class="sxs-lookup"><span data-stu-id="2d2e6-109">library</span></span>

<span data-ttu-id="2d2e6-110">Desuden vil lister, der bruger visse funktioner og tilpasninger, der ikke understøttes af moderne, stadig automatisk skifte til klassisk tilstand.</span><span class="sxs-lookup"><span data-stu-id="2d2e6-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="2d2e6-111">Startende 1, 2019, processen til deaktivering af det lejerniveau, du har logget af moderne liste og biblioteker, starter og fortsætter gennem maj 31, 2019.</span><span class="sxs-lookup"><span data-stu-id="2d2e6-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="2d2e6-112">De lister og biblioteker, der er i klassisk tilstand som resultat af lejerens lejer, bliver automatisk videre hævet til moderne.</span><span class="sxs-lookup"><span data-stu-id="2d2e6-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="2d2e6-113">Hvis du har brug for klassisk tilstand, skal du se flere oplysninger [her](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) og PnP PowerShell-instruktion [her](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) , der beskriver indstillinger og værktøjer, du kan bruge i dag for at bruge den klassiske oplevelse af tilstanden.</span><span class="sxs-lookup"><span data-stu-id="2d2e6-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
