---
title: Løs problemer med onboarding-Windows 10-enheder på Microsoft Defender Advanced Threat Protection
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 44969436c99b182cb4202fa60e2deb7d6ea3f460e48ee4649de1cfb646970f34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034028"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a>Løs problemer med onboarding-Windows 10-enheder på Microsoft Defender Advanced Threat Protection

Hvis du har adgang til fjerncomputeren, skal du følge disse trin:

1. Download [diagnosticeringsværktøjet Client Connectivity Analyzer.](https://go.microsoft.com/fwlink/?linkid=2143466)
2. Udtræk og kør MDATPAnalyzer.cmd.
3. Find diagnosticeringsloggen i mappen MDATPClientAnalyzerResult, som er den samme mappe, hvor analyseværktøjet blev hentet.
4. Hvis du vil finde problemer med forbindelsen eller internetproxyindstillingerne, skal du gennemse MDATPClientAnalyzer.txt.

Du kan få mere at vide [under Problemer med onboarding-maskiner.](https://go.microsoft.com/fwlink/?linkid=2143634)
