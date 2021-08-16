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
ms.openlocfilehash: f7b7e1ae4f1f686fa510403d398c4ff750dbadb9065b8d63701a927eeac52d9b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101296"
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

- Du er tildelt eksportrollen i Microsoft 365 Security &amp; Compliance Center. Som standard er denne rolle kun tildelt rollegruppen eDiscovery Manager. Se [Tildel eDiscovery-tilladelser](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

Få mere at vide under [Eksportér resultater fra indholdssøgning.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)

Hvis du eksporterer mere end 100.000 postkasser, skal du bruge følgende Powershell til at hente eksportresultaterne: Eksport af resultater fra mere end [100.000 postkasser.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)