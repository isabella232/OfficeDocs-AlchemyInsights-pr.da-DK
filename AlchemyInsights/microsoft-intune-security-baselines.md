---
title: Brug Microsoft Intune grundlinjer for sikkerhed til at konfigurere Windows 10 enheder
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: f77fdbb315db8317a6a1374f05489a7f5a0bedcec484dc9ac53a473098583949
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/11/2021
ms.locfileid: "57886626"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Brug Microsoft Intune grundlinjer for sikkerhed til at konfigurere Windows 10 enheder

Intune-sikkerhedsne grundlinjer hjælper med at beskytte brugere og enheder. Grundlinjer for sikkerhed er Windows forudkonfigurerede grupper, der bruges til at anvende en kendt gruppe af indstillinger og standardværdier anbefalet af de relevante sikkerhedsteams. Ved at oprette en profil for grundlinjer til sikkerhed i Intune kan du oprette en skabelon, der består af flere enhedskonfigurationsprofiler.

Når du installerer grundlinjer for sikkerhed for grupper af brugere eller enheder, anvendes indstillingerne på enheder, der kører på Windows 10 eller nyere. Sikkerheds baseline for Microsoft mobile device management (MDM) aktiverer f.eks. automatisk BitLocker til flytbare drev, kræver adgangskoden til at låse en enhed op og deaktiverer grundlæggende godkendelse. Når en standardværdi ikke fungerer for dit miljø, kan du tilpasse den oprindelige plan for at anvende de indstillinger, du har brug for.

Sikkerheds oprindelige planer hjælper også med at oprette en en sikker arbejdsproces i Microsoft 365. En grundlinje for sikkerhed indeholder de bedste fremgangsmåder og anbefalinger til indstillinger, der påvirker sikkerheden. Intune arbejder sammen med Windows, der opretter oprindelige planer for gruppepolitikker, så disse anbefalinger er baseret på solid vejledning og omfattende erfaring.

Hvis du er ny bruger af Intune og er usikker på, hvor du skal starte, hjælper sikkerheds oprindelige planer dig med hurtigt at oprette og implementere en sikker profil. Hvis du aktuelt bruger en gruppepolitik, er det meget nemmere at overføre til Intune til administrationsformål med sikkerheds oprindelige planer, fordi de er indbygget i Intune og indeholder avancerede administrationsfunktioner.

Du kan få mere at vide [Windows sikkerheds oprindelige planer](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) og Administration af [mobilenheder.](https://docs.microsoft.com/windows/client-management/mdm/)

