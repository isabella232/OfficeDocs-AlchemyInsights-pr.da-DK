---
title: Slå NDI-teknologi til
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004403"
- "7947"
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935083"
---
# <a name="turn-on-ndi-technology"></a><span data-ttu-id="c3405-102">Slå NDI-teknologi til</span><span class="sxs-lookup"><span data-stu-id="c3405-102">Turn on NDI technology</span></span>

<span data-ttu-id="c3405-103">NDI-teknologi kræver to trin for at være aktiveret for en bruger:</span><span class="sxs-lookup"><span data-stu-id="c3405-103">NDI technology requires two steps to be turned on for a user:</span></span>

1. <span data-ttu-id="c3405-104">Lejeradministratoren skal aktivere egenskaben 'AllowNDIStreaming' i CsTeamsMeetingPolicy.</span><span class="sxs-lookup"><span data-stu-id="c3405-104">The tenant admin must enable the 'AllowNDIStreaming' property in CsTeamsMeetingPolicy.</span></span>

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. <span data-ttu-id="c3405-105">Når denne ændring er udfyldt, skal slutbrugeren aktivere NDI®-teknologi for sin specifikke klient fra **Indstillinger > Tilladelser.**</span><span class="sxs-lookup"><span data-stu-id="c3405-105">After this change has populated, the end user must turn on NDI® technology for their specific client from **Settings > Permissions**.</span></span>

<span data-ttu-id="c3405-106">Du kan finde flere oplysninger [i Brug NDI-teknologi i Microsoft Teams.](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)</span><span class="sxs-lookup"><span data-stu-id="c3405-106">For more information, see [Use NDI technology in Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).</span></span>
