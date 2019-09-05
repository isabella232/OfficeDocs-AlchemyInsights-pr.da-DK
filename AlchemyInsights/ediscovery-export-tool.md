---
title: eksport værktøj til eDiscovery
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 8/3/2018
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
ms.openlocfilehash: 5a54344d43d16c77d440768aa1c87489edf10ca0
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736319"
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
  