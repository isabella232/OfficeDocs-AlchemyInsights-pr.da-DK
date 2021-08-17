---
title: Brug Microsoft Intune grundlinjer for sikkerhed til at konfigurere Windows 10 enheder
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: a94c6b72df3874ee80413adac86d60306175734b6ff28b2e015e05eec6f3838b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104338"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Brug Microsoft Intune grundlinjer for sikkerhed til at konfigurere Windows 10 enheder

Intune-sikkerheds oprindelige planer hjælper med at beskytte brugere og enheder. Sikkerheds baselines are Windows settings's forudkonfigurerede grupper, der bruges til at anvende en kendt gruppe af indstillinger og standardværdier anbefalet af de relevante sikkerhedsteams. Ved at oprette en profil for grundlinjer for sikkerheden i Intune kan du oprette en skabelon, der består af flere enhedskonfigurationsprofiler.

Når du installerer grundlinjer for sikkerhed for grupper af brugere eller enheder, anvendes indstillingerne på enheder, der kører på Windows 10 eller nyere. MdM Security Baseline (1) aktiverer f.eks. automatisk BitLocker til flytbare drev, (2) kræver adgangskoden til at låse en enhed op, og (3) deaktiverer grundlæggende godkendelse. Når en standardværdi ikke fungerer for dit miljø, kan du tilpasse den oprindelige plan for at anvende de indstillinger, du har brug for.

Sikkerheds oprindelige planer hjælper også med at oprette en en sikker arbejdsproces i Microsoft 365. Følgende er nogle af fordelene ved dette:

- En grundlinje for sikkerhed indeholder de bedste fremgangsmåder og anbefalinger til indstillinger, der påvirker sikkerheden. Da Intune samarbejder med Windows, der opretter oprindelige planer for gruppepolitikker, er disse anbefalinger baseret på solid vejledning og omfattende erfaring.
- Hvis du er ny bruger af Intune, og du ikke er sikker på, hvor du skal starte, kan sikkerheds oprindelige planer hjælpe dig med hurtigt at oprette og installere en sikker profil.
- Hvis du aktuelt bruger en gruppepolitik, er det meget nemmere at overføre til Intune til administrationsformål med sikkerheds oprindelige planer, fordi de er indbygget i Intune og indeholder avancerede funktioner til administration.

Du kan få mere at vide [Windows sikkerheds oprindelige planer](https://go.microsoft.com/fwlink/?linkid=2141503) og Administration af [mobilenheder.](https://go.microsoft.com/fwlink/?linkid=2141701)