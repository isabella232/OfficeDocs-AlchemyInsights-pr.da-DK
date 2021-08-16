---
title: Der returneres ingen resultater under indholdssøgning/-eksport
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
- "3200003"
- "7463"
ms.openlocfilehash: 5c04364f98dccbcad0f011df866f137d79c166ad3839b408d6be447d50a87ac3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101260"
---
# <a name="no-results-returned-during-content-searchexport"></a>Der returneres ingen resultater under indholdssøgning/-eksport

Hvis du oplever problemer med følgende eDiscovery-scenarier:

- Indholdssøgning/-eksport returnerer ingen data eller uventede data
- eDiscovery-søgning eller -eksport mislykkes

Dette kan skyldes visse sikkerhedsfiltre for overholdelse, der er konfigureret af en bestemt administrator, og som ikke er blevet kommunikeret til alle administratorer.

For at løse dette skal du kontrollere, om der er nogen sikkerhedsfiltre til overholdelse af regler og standarder, der kan være skyld i disse problemer:

1. Forbind til Security and Compliance Center Powershell
2. Kør følgende kommandoletter:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Du kan finde flere oplysninger om sikkerhedsfiltre til overholdelse af regler [og standarder under Filtrering af tilladelser til indholdssøgning](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
