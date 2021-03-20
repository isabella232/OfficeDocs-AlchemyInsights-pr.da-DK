---
title: Problemer med onboarding-maskiner til Microsoft Defender til slutpunkter
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901561"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a>Problemer med onboarding-maskiner til Microsoft Defender til slutpunkter

Der kan være problemer med onboarding-maskiner til MDE-tjenesten. Hvis du kan få adgang til slutbrugerens maskine, skal du følge disse trin:

1. Hent den nyeste prøveversion af diagnosticeringsværktøjet [MDE Client Analyzer.](https://aka.ms/betamdeanalyzer)
2. Højreklik på **MDEClientAnalyzer.cmd,** og vælg "Kør som administrator".
3. Følg eventuelle retningslinjer, der foreslås **iMDEClientAnalyzer.htm.**
4. Du kan finde flere detaljerede logfiler i den oprettede undermappe **MDEClientAnalyzerResult.**
5. Hvis yderligere vejledning er nødvendig, skal du [kontakte support til Microsoft Defender for Endpoint](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) og angive den MDEClientAnalyzerResult.zip fil til analyse.
