---
title: eDiscovery-eksportværktøj
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814582"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Kan du ikke installere eller køre eDiscovery-eksportværktøjet?

Hvis du ikke kan installere eller køre eDiscovery-eksportværktøjet for at hente søgeresultater, skal du kontrollere følgende:
  
- Den computer, du bruger, opfylder følgende forudsætninger:

  - 32- eller 64-bit versioner af Windows 7 og nyere versioner

  - Microsoft .NET Framework 4.7

  - En understøttet browser:

  - Microsoft Edge

    Eller

  - Internet Explorer 10 og nyere versioner

    Andre browsere, f.eks Google Chrome og Mozilla Firefox, understøttes ikke.

- Din organisation kan oprette forbindelse til slutpunktet i Azure, som er **\* .blob.core.windows.net** (jokertegnet repræsenterer et entydig identifier for dit eksportjob).

- Du er tildelt Eksport-rollen i Microsoft 365 Security &amp; Compliance Center. Som standard er denne rolle kun tildelt rollegruppen eDiscovery Manager. Se [Tildel eDiscovery-tilladelser](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

Få mere at vide under [Eksportér resultater fra indholdssøgning.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)

Hvis du eksporterer mere end 100.000 postkasser, skal du bruge følgende Powershell til at hente eksportresultaterne: Eksport af resultater fra mere end [100.000 postkasser.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)