---
title: EndPoint Manager – Grundlæggende sikkerhedsindstillinger
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
- "10064"
- "9003771"
ms.openlocfilehash: c13bc161b19a5fef1352beb28bdcc20110111a9a61a47433d82e1e69aff7f88d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53978155"
---
# <a name="endpoint-manager---security-baselines"></a>EndPoint Manager – Grundlæggende sikkerhedsindstillinger

Grundlæggende sikkerhedsindstillinger er forudkonfigurerede grupper af Windows-indstillinger, der hjælper dig med at anvende de sikkerhedsindstillinger, der anbefales af de relevante sikkerhedsteams. Disse grundindstillinger kan tilpasses, så de udelukkende leverer de ønskede indstillinger og værdier. Du kan finde flere oplysninger om de grundlæggende sikkerhedsindstillinger under [Brug grundlæggende sikkerhedsindstillinger til at konfigurere Windows 10-enheder i Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).

Der er i øjeblikket grundindstillinger for disse produkter:

- Sikkerhedsindstillinger for Windows MDM
- Microsoft Defender for Endpoint Security
- Microsoft Edge

Hver grundindstilling opdateres med jævne mellemrum og udgives i trinvise versioner. Hver version tilføjer og eller fjerner indstillinger fra den tidligere version for at sikre, at grundindstillingen opfylder den aktuelle vejledning. De grundlæggende sikkerhedsindstillinger i Endpoint Security gør det muligt at sammenligne forskellige versioner ved at foretage ændringer fra version til version synlig. 

Du kan få vejledning til, hvordan du mest effektivt ændrer, hvilken version af grundindstilling, der installeres, i [Administrer profiler for grundlæggende sikkerhedsindstillinger i Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).

Når du har udrullet en grundlæggende sikkerhedsindstilling, kan du overvåge dens aktiverede tilstand og gennemse indstillingerne fra enhed til enhed.

**Bemærk:** Det kan tage op til 24 timer, før rapporteringsdataene for grundlæggende sikkerhedsindstillinger vises efter den første installation på en enhed og op til 6 timer for yderligere opdateringer. 

Den mest almindelige årsag til, at en grundindstilling ikke anvendes, er, at den samme indstilling bruges i en anden profil. Dette scenarie kan undersøges for en bestemt enhed ved at vælge den pågældende enhed i enhedens statusnode på profilen Grundlæggende sikkerhedsindstillinger. For flere detaljer, se [Løs konflikter for grundlæggende sikkerhedsindstillinger](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).