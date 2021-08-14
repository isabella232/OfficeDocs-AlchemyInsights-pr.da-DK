---
title: Programbeskyttelsespolitik
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
ms.openlocfilehash: ab6ad9c4bf95ee013c66384ec8449ceb1b56e8f3ea9e95c695dbbab0e9fa3fc3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53969965"
---
# <a name="application-protection-policy"></a>Programbeskyttelsespolitik

Hvis du er ny bruger af Programbeskyttelsespolitik (APP), skal du se Oversigt over [politikker for beskyttelse af apps](https://docs.microsoft.com/intune/apps/app-protection-policy).

Hvis du vil begynde at bruge APP, skal [du se Sådan opretter og tildeler du beskyttelsespolitikker for apps.](https://docs.microsoft.com/intune/app-protection-policies)

Krav til programbeskyttelsespolitik:

- Brugeren har en Intune- eller EMS-licens.
- Brugeren tilhører en gruppe, der er målrettet efter politikker for programbeskyttelse.
- Kun én virksomhedsbruger er logget på beskyttede apps på en enhed.
- Programmet har implementeret [Intune SDK.](https://docs.microsoft.com/intune/app-sdk-get-started) Du kan finde en liste over apps, der understøtter SDK, [Microsoft Intune beskyttede apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).

Politikker gælder, når en bruger, der opfylder ovenstående krav, logger på en app, der er aktiveret af Intune SDK. Den nemmeste måde at afgøre, om en politik anvendes, er ved at kræve, at brugeren angiver en pinkode i politikken. 

Du kan finde flere oplysninger under:

[Ofte stillede spørgsmål om APP/MAM-fejlfinding](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[Sådan validerer du konfigurationen af din app-beskyttelsespolitik](https://docs.microsoft.com/intune/app-protection-policies-validate)

[Forstå tidsindstilling for levering af appbeskyttelsespolitik](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[Sådan overvåges politikker for appbeskyttelse](https://docs.microsoft.com/intune/app-protection-policies-monitor)