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
# <a name="turn-on-ndi-technology"></a>Slå NDI-teknologi til

NDI-teknologi kræver to trin for at være aktiveret for en bruger:

1. Lejeradministratoren skal aktivere egenskaben 'AllowNDIStreaming' i CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Når denne ændring er udfyldt, skal slutbrugeren aktivere NDI®-teknologi for sin specifikke klient fra **Indstillinger > Tilladelser.**

Du kan finde flere oplysninger [i Brug NDI-teknologi i Microsoft Teams.](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)
