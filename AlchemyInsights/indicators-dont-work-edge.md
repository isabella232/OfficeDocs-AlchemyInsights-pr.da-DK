---
title: Symboler fungerer ikke ved hjælp af Microsoft Edge-browseren
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676132"
---
# <a name="indicators-dont-work-using-edge-browser"></a>Symboler fungerer ikke ved hjælp af Microsoft Edge-browseren

Når du har oprettet en indikator, bliver den ikke imødekommet af Edge (SmartScreen). Få mere at vide under [Opret indikatorer for IP'er og URL-adresser/domæner.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)

## <a name="step-1-ensure-the-following"></a>Trin 1: Sørg for følgende

- Kontrollér, at indikatoren er korrekt (ingen slåfejl i IP/URL, korrekt handling, de korrekte RBAC-grupper).
- Vent mindst 2 timer efter oprettelse af indikatoren for at tage højde for enhver mulig ventetid.
- Kontrollér, at systemet/systemerne er onboardet til Microsoft Defender til slutpunkt.
- Kontrollér, at systemer kan kommunikere med skyen.
- Kontrollér, at Smartscreen er aktiveret og tilgængelig ved at gå til [testwebstedet.](https://demo.smartscreen.msft.net)

## <a name="step-2-troubleshoot-the-potential-issue"></a>Trin 2: Fejlfinding af det potentielle problem

- Kontrollér, at klienten opfylder kravene. Du kan få mere at [vide under Oprette indikatorer for IP'er og URL-adresser/domæner.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)
- Sørg for, at du kører den nyeste version af Edge-browseren. Hvis du vil finde ud af den nyeste version, [skal du se Find ud af, hvilken version Microsoft Edge du har.](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)
- Genstart Edge-browseren.
- Gå til det websted, hvor du har konfigureret en indikator. Hvis webstedet ikke vises som forventet, skal du fortsætte til trin 3. 

## <a name="step-3-collect-data"></a>Trin 3: Indsaml data

- **Indsaml diagnostiske MDEClientAnalyzer-data.** Du kan finde en vejledning [under Problemer med onboardingmaskine til Microsoft Defender til slutpunkt.](issues-with-onboarding-machines.md)
- Hvis du er tryg ved at installere og indsamle en Fiddler-sporing, skal du [se Telerik Fiddler](http://www.telerik.com/fiddler).
- Hvis du foretrækker vejledning fra Microsoft Support, kan du vælge ikonet Support nedenfor for at åbne en supportsag.
