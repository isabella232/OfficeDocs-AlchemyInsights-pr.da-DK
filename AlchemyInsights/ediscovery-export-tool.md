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
ms.openlocfilehash: 83f18d06006989e03ee6095e430aaf3eb5c72c09
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714764"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Kan du ikke installere eller køre eDiscovery Export Tool?

Hvis du ikke kan installere eller køre eDiscovery Export Tool for at hente søgeresultater, skal du kontrollere følgende:
  
- Den computer, du bruger, opfylder disse forudsætninger:

  - 32- eller 64-bit versioner af Windows 7 og nyere versioner

  - Microsoft .NET Framework 4.7

  - En understøttet browser:

  - Microsoft Edge

    Eller

  - Internet Explorer 10 og nyere versioner

    Andre browsere, såsom Google Chrome og Mozilla Firefox understøttes ikke.

- Din organisation kan oprette forbindelse til slutpunktet i Azure, som er ** \*.blob.core.windows.net** (jokertegnet repræsenterer et entydigt id for dit eksportjob).

- Du tildeles rollen Eksporter i Microsoft &amp; 365 Security Compliance Center. Denne rolle tildeles som standard kun til rollegruppen eDiscovery Manager. Se [Tildele eDiscovery-tilladelser](https://docs.microsoft.com/office365/securitycompliance/assign-ediscovery-permissions).

Yderligere oplysninger finder du i [Export Content Search Results](https://docs.microsoft.com/office365/securitycompliance/export-search-results).
  