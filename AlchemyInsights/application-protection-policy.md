---
title: Politik for beskyttelse af programmer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/22/2020
ms.locfileid: "45423431"
---
# <a name="application-protection-policy"></a>Politik for beskyttelse af programmer

Hvis du er ny bruger af App(Application Protection Policy), kan du se [oversigten over politikker for appbeskyttelse](https://docs.microsoft.com/intune/apps/app-protection-policy).

Hvis du vil begynde at bruge APP, [skal du se Sådan oprettes og tildeles politikker for appbeskyttelse](https://docs.microsoft.com/intune/app-protection-policies).

Krav til politikken for beskyttelse af programmer:

- Brugeren har en Intune- eller EMS-licens.
- Brugeren tilhører en gruppe, der er målrettet mod programbeskyttelsespolitikker.
- Kun én virksomhedsbruger er logget på beskyttede apps på en enhed.
- Ansøgningen har implementeret [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started). Du kan finde en liste over apps, der understøtter SDK, i [Microsoft Intune-beskyttede apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).

Politikker gælder, når en bruger, der opfylder ovenstående krav, logger på en Intune SDK-aktiveret app. Den nemmeste måde at afgøre, om en politik anvendes, er ved at kræve, at brugeren angiver en nål i politikken. 

Du kan finde flere oplysninger under:

[Ofte stillede spørgsmål om fejlfinding af APP/MAM](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[Sådan validerer du konfigurationen af din politik for appbeskyttelse](https://docs.microsoft.com/intune/app-protection-policies-validate)

[Forstå leveringstidstidspunktet for appbeskyttelsespolitik](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[Sådan overvåges politikker for appbeskyttelse](https://docs.microsoft.com/intune/app-protection-policies-monitor)