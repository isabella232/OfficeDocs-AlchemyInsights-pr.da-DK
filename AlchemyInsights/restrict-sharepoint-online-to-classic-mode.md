---
title: Begrænse SharePoint Online til tilstanden Klassisk
ms.author: kirks
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
ms.openlocfilehash: e7ecfd8c2f1a532355bfb8c2c0a846fc0d6e88b1
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551553"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="9aebf-102">Begrænse SharePoint Online til tilstanden Klassisk</span><span class="sxs-lookup"><span data-stu-id="9aebf-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="9aebf-103">Nogle organisationer kræver stadig klassisk tilstand oplevelse.</span><span class="sxs-lookup"><span data-stu-id="9aebf-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="9aebf-104">Der er ingen planer om at fjerne klassiske tilstand på et detaljeret niveau, der ikke længere muligt at begrænse en hel organisation (lejer) til klassisk tilstand for lister og biblioteker.</span><span class="sxs-lookup"><span data-stu-id="9aebf-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="9aebf-105">Administratoren har følgende indstillinger til at administrere individuelle lister og biblioteker i classic-tilstand ved hjælp af detaljeret fravalg af parametre, som vi giver på følgende niveauer:</span><span class="sxs-lookup"><span data-stu-id="9aebf-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="9aebf-106">gruppe af websteder</span><span class="sxs-lookup"><span data-stu-id="9aebf-106">site collection</span></span>
- <span data-ttu-id="9aebf-107">websted</span><span class="sxs-lookup"><span data-stu-id="9aebf-107">site</span></span>
- <span data-ttu-id="9aebf-108">liste</span><span class="sxs-lookup"><span data-stu-id="9aebf-108">list</span></span>
- <span data-ttu-id="9aebf-109">bibliotek</span><span class="sxs-lookup"><span data-stu-id="9aebf-109">library</span></span>

<span data-ttu-id="9aebf-110">Derudover bliver lister, som du kan bruger visse funktioner og tilpasninger, der ikke understøttes af moderne stadig automatisk ændres til klassisk tilstand.</span><span class="sxs-lookup"><span data-stu-id="9aebf-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="9aebf-111">Begyndende April 1, 2019, proces for at deaktivere niveauet lejer framelde moderne liste og biblioteker starter og fortsætte gennem 31 maj 2019.</span><span class="sxs-lookup"><span data-stu-id="9aebf-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="9aebf-112">Lister og biblioteker, der er i klassisk tilstand som følge af fravalg af lejer vil automatisk flyttes til moderne.</span><span class="sxs-lookup"><span data-stu-id="9aebf-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="9aebf-113">Hvis du har brug for klassisk tilstand finder du yderligere oplysninger [her](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) , og PnP Powershell instruktion [her](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) , der beskriver indstillinger og værktøjer, du kan bruge i dag til at bruge tilstanden Klassisk-oplevelse.</span><span class="sxs-lookup"><span data-stu-id="9aebf-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
