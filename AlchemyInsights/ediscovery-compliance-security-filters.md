---
title: Ingen resultater returneret under indholdssøgning/eksport
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
ms.openlocfilehash: 8786f11f170edb151879235e19caa38b50f3f06e
ms.sourcegitcommit: 3d662e1a1440ba74b5347896347d03bb8c8f3af5
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/22/2020
ms.locfileid: "49727217"
---
# <a name="no-results-returned-during-content-searchexport"></a>Ingen resultater returneret under indholdssøgning/eksport

Hvis du oplever problemer med følgende eDiscovery-scenarier:

- Indholdssøgning/eksport returnerer ingen data eller uventede data
- eDiscovery-søgning eller eksport mislykkes

Dette kan skyldes visse sikkerhedsfiltre for overholdelse, der blev oprettet af en bestemt administrator, og som ikke er blevet kommunikeret med alle administratorer.

Hvis du vil løse dette, skal du kontrollere, om der er nogen sikkerhedsfiltre for overholdelse, der kan forårsage disse problemer:

1. Opret forbindelse til sikkerheds-og overholdelses Center PowerShell
2. Kør følgende commandlets:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Du kan finde flere oplysninger om kompatibilitets relaterede filtre under [tilladelser til filtrering af indholdssøgning](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
