---
title: Brug microsoft Intune-sikkerheds oprindelige planer til konfiguration af Windows 10-enheder
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50693414"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a>Brug microsoft Intune-sikkerheds oprindelige planer til konfiguration af Windows 10-enheder

Intune-sikkerheds baselines hjælper med at beskytte brugere og enheder. Sikkerheds baselines are Windows settings'pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams. Ved at oprette en profil for grundlinjer til sikkerhed i Intune kan du oprette en skabelon, der består af flere enhedskonfigurationsprofiler.

Når du installerer grundlinjer til sikkerhed for grupper af brugere eller enheder, anvendes indstillingerne på enheder, der kører på Windows 10 eller nyere versioner. Sikkerheds baseline (1) for Microsoft Mobile Device Management (MDM) aktiverer f.eks. automatisk BitLocker til flytbare drev (2) kræver adgangskoden til åbning af en enhed, og (3) deaktiverer grundlæggende godkendelse. Når en standardværdi ikke fungerer for dit miljø, kan du tilpasse den oprindelige plan for at anvende de indstillinger, du har brug for.

Sikkerheds baselines also help establish an end-to-end secure workflow in Microsoft 365. Følgende er nogle af fordelene ved denne funktionalitet:
- En grundlinje for sikkerhed omfatter de bedste fremgangsmåder og anbefalinger til indstillinger, der påvirker sikkerheden. Da Intune samarbejder med Windows-sikkerhedsteamet, der opretter grundlinjer for gruppepolitikker, er disse anbefalinger baseret på solid vejledning og omfattende erfaring.
- Hvis du er ny bruger af Intune og er usikker på, hvor du skal starte, kan sikkerheds oprindelige planer hjælpe dig med hurtigt at oprette og installere en sikker profil.
- Hvis du i øjeblikket bruger en gruppepolitik, er det meget nemmere at overføre til Intune til administrationsformål med sikkerheds oprindelige planer, fordi disse sikkerheds oprindelige planer er indbygget i Intune og indeholder avancerede funktioner til administration.

Du kan finde flere oplysninger i [Windows-sikkerhedsscenarier](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) [og administration af mobilenheder.](https://docs.microsoft.com/windows/client-management/mdm/)