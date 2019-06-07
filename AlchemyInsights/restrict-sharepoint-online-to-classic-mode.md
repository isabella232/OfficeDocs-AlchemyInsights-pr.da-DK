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
ms.openlocfilehash: 76f0b5ed67d3220559d25dfd72c7535181a4513b
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/07/2019
ms.locfileid: "34761753"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="0f056-102">Begrænse SharePoint Online til tilstanden Klassisk</span><span class="sxs-lookup"><span data-stu-id="0f056-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="0f056-103">Nogle organisationer kræver stadig klassisk tilstand oplevelse.</span><span class="sxs-lookup"><span data-stu-id="0f056-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="0f056-104">Der er ingen planer om at fjerne klassiske tilstand på et detaljeret niveau, der ikke længere muligt at begrænse en hel organisation (lejer) til klassisk tilstand for lister og biblioteker.</span><span class="sxs-lookup"><span data-stu-id="0f056-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="0f056-105">Administratoren har følgende indstillinger til at administrere individuelle lister og biblioteker i classic-tilstand ved hjælp af detaljeret fravalg af parametre, som vi giver på følgende niveauer:</span><span class="sxs-lookup"><span data-stu-id="0f056-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="0f056-106">gruppe af websteder</span><span class="sxs-lookup"><span data-stu-id="0f056-106">site collection</span></span>
- <span data-ttu-id="0f056-107">websted</span><span class="sxs-lookup"><span data-stu-id="0f056-107">site</span></span>
- <span data-ttu-id="0f056-108">liste</span><span class="sxs-lookup"><span data-stu-id="0f056-108">list</span></span>
- <span data-ttu-id="0f056-109">bibliotek</span><span class="sxs-lookup"><span data-stu-id="0f056-109">library</span></span>

<span data-ttu-id="0f056-110">Derudover bliver lister, som du kan bruger visse funktioner og tilpasninger, der ikke understøttes af moderne stadig automatisk ændres til klassisk tilstand.</span><span class="sxs-lookup"><span data-stu-id="0f056-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="0f056-111">Begyndende April 1, 2019, proces for at deaktivere niveauet lejer framelde moderne liste og biblioteker starter og fortsætte gennem 31 maj 2019.</span><span class="sxs-lookup"><span data-stu-id="0f056-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="0f056-112">Lister og biblioteker, der er i klassisk tilstand som følge af fravalg af lejer vil automatisk flyttes til moderne.</span><span class="sxs-lookup"><span data-stu-id="0f056-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="0f056-113">Hvis du har brug for klassisk tilstand finder du yderligere oplysninger [her](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) , og PnP Powershell instruktion [her](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) , der beskriver indstillinger og værktøjer, du kan bruge i dag til at bruge tilstanden Klassisk-oplevelse.</span><span class="sxs-lookup"><span data-stu-id="0f056-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
