---
title: eksport værktøj til eDiscovery
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
ms.openlocfilehash: 7e2964ef0a44ddf421e4aae007acbdbda196e20f
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/29/2019
ms.locfileid: "37769297"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Kan du ikke installere eller køre værktøjet eDiscovery Export?

Hvis du ikke kan installere eller køre Office 365 eDiscovery-eksportværktøjet for at hente søgeresultater, skal du kontrollere følgende:
  
- Den computer, du bruger, opfylder disse forudsætninger:

  - 32-eller 64-bit versioner af Windows 7 og nyere versioner

  - Microsoft .NET Framework 4,7

  - En understøttet browser:

  - Microsoft Edge

    Eller

  - Internet Explorer 10 og nyere versioner

    Andre browsere, såsom Google Chrome og Mozilla Firefox, understøttes ikke.

- Din organisation kan oprette forbindelse til slutpunktet i Azure, som er ** \*. blob.Core.Windows.net** (jokertegnet repræsenterer et entydigt id for eksportjobbet).

- Du er tildelt eksport rollen i Office 365 Security &amp; Compliance Center. Rollen tildeles som standard kun til rollegruppen eDiscovery Manager. Se [tildele eDiscovery-tilladelser](https://docs.microsoft.com/office365/securitycompliance/assign-ediscovery-permissions).

Du finder flere oplysninger i [eksportere indholds søgeresultater](https://docs.microsoft.com/office365/securitycompliance/export-search-results).
  