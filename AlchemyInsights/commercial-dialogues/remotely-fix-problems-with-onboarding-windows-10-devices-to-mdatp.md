---
title: Løs problemer med onboarding af Windows 10-enheder fra en fjernforbindelse til Microsoft Defender Advanced Threat Protection
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
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744720"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a>Løs problemer med onboarding af Windows 10-enheder fra en fjernforbindelse til Microsoft Defender Advanced Threat Protection

Hvis du kan få adgang til fjerncomputeren, skal du følge disse trin:

1. Download [diagnosticeringsværktøjet Client Connectivity Analyzer.](https://go.microsoft.com/fwlink/?linkid=2143466)
2. Udtræk og kør MDATPAnalyzer.cmd.
3. Find diagnosticeringsloggen i mappen MDATPClientAnalyzerResult, som er den samme mappe, hvor analyseværktøjet blev hentet.
4. Hvis du vil finde problemer med forbindelses- eller internetproxyindstillingerne, skal du gennemse MDATPClientAnalyzer.txt.

Du kan få mere at vide [under Problemer med onboarding-maskiner.](https://go.microsoft.com/fwlink/?linkid=2143634)
