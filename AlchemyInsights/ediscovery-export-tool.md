---
title: eDiscovery-eksportværktøj
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 6352603a391ddcb44d2728c7587bf15a6cd97ebb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507164"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Kan du ikke installere eller køre eDiscovery Export Tool?

Hvis du ikke kan installere eller køre eDiscovery-eksportværktøjet for at hente søgeresultater, skal du kontrollere følgende:
  
- Den computer, du bruger, opfylder disse forudsætninger:

  - 32- eller 64-bit versioner af Windows 7 og nyere versioner

  - Microsoft .NET Framework 4.7

  - En understøttet browser:

  - Microsoft Edge

    Eller

  - Internet Explorer 10 og nyere versioner

    Andre browsere, f.eks.

- Din organisation kan oprette forbindelse til slutpunktet i Azure, som er ** \* .blob.core.windows.net** (jokertegnet repræsenterer et entydigt id for dit eksportjob).

- Du tildeler eksportrollen i Microsoft 365 Security &amp; Compliance Center. Denne rolle tildeles som standard kun til rollegruppen eDiscovery Manager. Se [Tildele eDiscovery-tilladelser](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

Du kan finde flere oplysninger under [Eksportere søgeresultater for indhold](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).
  