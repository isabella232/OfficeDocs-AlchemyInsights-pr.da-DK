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
ms.openlocfilehash: c51e48fe5694f964aef74c2973f774b44415ebb8
ms.sourcegitcommit: 21cfb213183188d32a3743f66db10a8463019965
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/28/2019
ms.locfileid: "30955977"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="6419c-102">Begrænse SharePoint Online til tilstanden Klassisk</span><span class="sxs-lookup"><span data-stu-id="6419c-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="6419c-103">Nogle organisationer kræver stadig klassisk tilstand oplevelse.</span><span class="sxs-lookup"><span data-stu-id="6419c-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="6419c-104">Der er ingen planer om at fjerne klassiske tilstand på et detaljeret niveau, Start April 1,2019, vil det ikke længere være muligt at begrænse en hel organisation (lejer) til klassisk tilstand for lister og biblioteker.</span><span class="sxs-lookup"><span data-stu-id="6419c-104">While there are no plans to remove classic mode at a granular level, starting April 1,2019, it will no longer be possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="6419c-105">Administratoren har følgende indstillinger til at administrere individuelle lister og biblioteker i classic-tilstand ved hjælp af detaljeret fravalg af parametre, som vi giver på følgende niveauer:</span><span class="sxs-lookup"><span data-stu-id="6419c-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="6419c-106">gruppe af websteder</span><span class="sxs-lookup"><span data-stu-id="6419c-106">site collection</span></span>
- <span data-ttu-id="6419c-107">websted</span><span class="sxs-lookup"><span data-stu-id="6419c-107">site</span></span>
- <span data-ttu-id="6419c-108">liste</span><span class="sxs-lookup"><span data-stu-id="6419c-108">list</span></span>
- <span data-ttu-id="6419c-109">bibliotek</span><span class="sxs-lookup"><span data-stu-id="6419c-109">library</span></span>

<span data-ttu-id="6419c-110">Derudover bliver lister, som du kan bruger visse funktioner og tilpasninger, der ikke understøttes af moderne stadig automatisk ændres til klassisk tilstand.</span><span class="sxs-lookup"><span data-stu-id="6419c-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="6419c-111">Efter 1. April, vil lister og biblioteker, der er i klassisk tilstand som følge af fravalg af lejer automatisk blive håndteret på webstedsniveau og niveau.</span><span class="sxs-lookup"><span data-stu-id="6419c-111">After April 1, lists and libraries that are in classic mode as a result of tenant opt-out will automatically be managed at the site level and list level.</span></span>

<span data-ttu-id="6419c-112">Hvis du har brug for klassisk tilstand du finder yderligere oplysninger her, og PnP Powershell instruktion her, der beskriver indstillinger og værktøjer, du kan bruge i dag til at forberede til fjernelse af de lejer niveau fravælge d. 1.</span><span class="sxs-lookup"><span data-stu-id="6419c-112">If you require classic mode please see more information here and PnP Powershell instruction here that describes options and tools you can use today to prepare for the removal of the tenant level opt-out on April 1.</span></span>
