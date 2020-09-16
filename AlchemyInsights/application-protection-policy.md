---
title: Politik for beskyttelse af programmer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 929400dcf0ca18ce8f52cb11e5c907064449480e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47716887"
---
# <a name="application-protection-policy"></a>Politik for beskyttelse af programmer

Hvis du er ny for program beskyttelsespolitik (APP), skal du se [Oversigt over politikker for app-beskyttelse](https://docs.microsoft.com/intune/apps/app-protection-policy).

Hvis du vil begynde at bruge APPEN, skal du se [Sådan oprettes og tildeles politikker for app-beskyttelse](https://docs.microsoft.com/intune/app-protection-policies).

Krav til politik for beskyttelse af programmer:

- Brugeren har en Intune-eller EMS-licens.
- Brugeren tilhører en gruppe, der er målrettet mod politikker for beskyttelse af programmer.
- Kun én erhvervsbruger er logget på beskyttede apps på en enhed.
- Programmet har implementeret [INTUNE SDK](https://docs.microsoft.com/intune/app-sdk-get-started). Du kan finde en liste over apps, der understøtter SDK, under [Microsoft Intune-beskyttede apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).

Politikker gælder, når en bruger, der opfylder ovenstående krav, logger på en Intune SDK-aktiveret app. Den nemmeste måde at finde ud af, om en politik anvendes, er ved at kræve, at brugeren angiver en pinkode i politikken. 

Du kan finde flere oplysninger under:

[Ofte stillede spørgsmål om fejlfinding af apps/MAM](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[Sådan validerer du konfigurationen af politik for app-beskyttelse](https://docs.microsoft.com/intune/app-protection-policies-validate)

[Forstå timing for levering af politik for app-beskyttelse](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[Sådan overvåges politikker for app-beskyttelse](https://docs.microsoft.com/intune/app-protection-policies-monitor)