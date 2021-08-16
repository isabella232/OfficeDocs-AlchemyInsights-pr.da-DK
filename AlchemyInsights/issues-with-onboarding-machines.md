---
title: Problemer med onboardingmaskine til Microsoft Defender til slutpunkter
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
ms.openlocfilehash: 5f2ed08e32694a6d7293abbabb1eddd3d251ceddbd9debf6ec3143bb4fed86db
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054684"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a>Problemer med onboardingmaskine til Microsoft Defender til slutpunkter

Der kan være problemer med onboardingmaskine til MDE-tjenesten. Hvis du kan få adgang til slutbrugerens maskine, skal du følge disse trin:

1. Download den nyeste prøveversion af [diagnosticeringsværktøjet MDE Client Analyzer.](https://aka.ms/betamdeanalyzer)
2. Højreklik på **MDEClientAnalyzer.cmd,** og vælg "Kør som administrator".
3. Følg eventuelle retningslinjer, der foreslås **iMDEClientAnalyzer.htm**.
4. Se den oprettede undermappe **MDEClientAnalyzerResult** for at få flere detaljerede logfiler.
5. Hvis yderligere vejledning er nødvendig, skal [du kontakte support til Microsoft Defender for Endpoint](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) og angive den MDEClientAnalyzerResult.zip fil til analyse.
