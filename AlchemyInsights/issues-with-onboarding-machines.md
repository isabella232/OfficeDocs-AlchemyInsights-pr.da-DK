---
title: Problemer med onboardingmaskiner
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/15/2020
ms.locfileid: "45141365"
---
# <a name="issues-with-onboarding-machines"></a>Problemer med onboardingmaskiner

Du har muligvis problemer med onboardingmaskiner til MDATP-tjenesten. Hvis du har adgang til slutbrugermaskinen, skal du følge disse trin:

1. Hent [diagnosticeringsværktøjet Client Connectivity Analyzer.](https://aka.ms/mdatpanalyzer)
2. Udtræk og kør MDATPAnalyzer.cmd.
3. Find diagnosticeringsloggen i mappen MDATPClientAnalyzerResult, den samme mappe, hvor værktøjet Analysator hentes.
4. Gennemse logfilen, MDATPClientAnalyzer.txt, for at finde problemer med forbindelses- eller internetproxyindstillinger.