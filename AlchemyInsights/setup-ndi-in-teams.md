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
ms.openlocfilehash: ed932592aae1158bc0c0da4817467b69d20208533bc080cb0e424f552af8601a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54023516"
---
# <a name="turn-on-ndi-technology"></a>Slå NDI-teknologi til

NDI-teknologi kræver to trin for at være aktiveret for en bruger:

1. Lejeradministratoren skal aktivere egenskaben "AllowNDIStreaming" i CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Når denne ændring er blevet udfyldt, skal slutbrugeren aktivere NDI®-teknologi for deres specifikke **klient Indstillinger > Tilladelser.**

Du kan finde flere oplysninger [under Brug NDI-teknologi i Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).
