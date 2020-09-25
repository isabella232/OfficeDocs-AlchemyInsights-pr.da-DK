---
title: eDiscovery-eksport værktøj
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277938"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Kan du ikke installere eller køre eDiscovery-eksport værktøj?

Hvis du ikke kan installere eller køre eDiscovery-eksportværktøjet for at hente søgeresultater, skal du kontrollere følgende:
  
- Den computer, du bruger, opfylder følgende forudsætninger:

  - 32-eller 64-bit versioner af Windows 7 og nyere versioner

  - Microsoft .NET Framework 4.7

  - En understøttet browser:

  - Microsoft Edge

    Eller

  - Internet Explorer 10 og nyere versioner

    Andre browsere, f. eks Google Chrome og Mozilla Firefox, understøttes ikke.

- Din organisation kan oprette forbindelse til slutpunktet i Azure, som er ** \* . blob.Core.Windows.net** (jokertegnet repræsenterer et entydigt id for dit eksport-job).

- Du er tildelt eksport rollen i Microsoft 365 Security &amp; Compliance Center. Denne rolle tildeles som standard kun rollegruppen eDiscovery Manager. Se [Tildel eDiscovery-tilladelser](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

Hvis du vil have mere at vide, skal du se [eksportere resultater for indholdssøgning](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).

Hvis du eksporterer mere end 100K-postkasser, skal du bruge følgende PowerShell til at downloade eksportresultaterne:  [eksportere resultater fra mere end 100K postkasser](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).