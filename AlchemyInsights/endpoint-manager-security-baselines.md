---
title: EndPoint Manager – grundlinjer for sikkerhed
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
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/29/2021
ms.locfileid: "51420774"
---
# <a name="endpoint-manager---security-baselines"></a>EndPoint Manager – grundlinjer for sikkerhed

Sikkerheds baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams. Disse oprindelige planer kan tilpasses, så de kun leverer de ønskede indstillinger og værdier. Du kan finde flere oplysninger om grundlinjer for sikkerhed under Brug af sikkerheds oprindelige planer til konfiguration af [Windows 10-enheder i Intune.](https://docs.microsoft.com/mem/intune/protect/security-baselines)

Der er i øjeblikket grundlinjer for disse produkter:

- Sikkerhedsindstillinger for Windows MDM
- Microsoft Defender for EndPoint Security
- Microsoft Edge

Hver af de oprindelige planer opdateres med jævne mellemrum og udgives i trinvise versioner. Hver version tilføjer og fjerner indstillinger fra den forrige version for at sikre, at den oprindelige plan opfylder den aktuelle vejledning. Konsollen sikkerhedsmæssige grundlinjer i Slutpunktssikkerhed gør det muligt at sammenligne forskellige versioner ved at gøre ændringerne fra version til version synlige.

Du kan finde en vejledning til, hvordan du mest effektivt kan ændre, hvilken version af den oprindelige plan der installeres, under Administrere profiler for oprindelige [sikkerhed i Microsoft Intune.](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)

Når du har implementeret en grundlinje for sikkerhed, kan du overvåge installationstilstanden og gennemse indstillingerne på enhed for enhed.

**Bemærk!** Det kan tage op til 24 timer, før data for oprindelige planer vises fra installationsstart til en enhed og op til 6 timer for yderligere opdateringer. 

Den mest almindelige årsag til, at en oprindelig plan ikke anvendes, er, at den samme indstilling bruges i en anden profil. Dette scenarie kan undersøges for en bestemt enhed ved at vælge enheden i knudepunktet Enhedsstatus i profilen Grundlinje for sikkerhed. Du kan finde flere oplysninger [i Løse konflikter for sikkerheds oprindelige planer.](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)