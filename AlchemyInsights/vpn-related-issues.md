---
title: VPN-relaterede problemer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 1d9c34350d16d96329d1ed56666119dba0433c93ccb7547da5dba4894531e1b4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53970973"
---
# <a name="vpn-related-issues"></a>VPN-relaterede problemer

En vellykket implementering af VPN-forbindelsen for MDM-klienter afhænger af en installeret profil, der korrekt afspejler kravene til VPN-infrastrukturen. Du kan finde de relevante indstillinger for de klientplatforme, du undersøger, i: 

[Windows 10 og Windows holografiske enhedsindstillinger for at tilføje VPN-forbindelser ved hjælp af Intune](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[Tilføj VPN-indstillinger på iOS- og iPadOS-enheder i Microsoft Intune](https://docs.microsoft.com/intune/vpn-settings-ios)  
[Indstillinger for Android-enhed til konfiguration af VPN i Intune](https://docs.microsoft.com/intune/vpn-settings-android)  
[Tilføj VPN-indstillinger på macOS-enheder i Microsoft Intune](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

Hvis din VPN-profil bruger certifikatbaseret godkendelse, skal du sørge for, at rodcertifikatet og klientgodkendelsescertifikatprofiler, der er knyttet til VPN-profilen, er installeret korrekt.

**Almindelige problemer**

**Jeg har installeret en VPN-profil på en enhed. Intune viser, at det lykkedes, men enheden opretter ikke forbindelse til VPN.**

En vellykket status betyder, at Intune har installeret profilen som konfigureret. Disse konfigurationer opfylder dog muligvis ikke dine krav til netværk og/eller godkendelse. Gennemgå loggene i infrastruktur og autentifikationsservice (på VPN-serveren og NPS/Radius-serveren) for at få flere oplysninger om den forsøgte forbindelse. Du skal muligvis arbejde med dit netværksinfrastrukturteam eller tredjeparts VPN-leverandøren for at indsamle og gennemgå logfiler.

**Når jeg konfigurerer et brugerdefineret VPN til iOS, bliver VPN-funktionen pr. app ikke tilgængelig.**

VPN pr. app til iOS-enheder i Intune er i øjeblikket tilgængeligt for en specifik liste over udbydere og partnere, som også skal opfylde certifikatfor forudsætningerne, før du konfigurerer et VPN pr. app. Du kan få mere at vide under Konfigurer virtuelt privat netværk [pr. app (VPN) til iOS-/iPadOS-enheder i Intune.](https://docs.microsoft.com/intune/vpn-setting-configure-per-app) 

Du kan finde flere oplysninger om alle VPN-forbindelsestyper i Intune i Opret VPN-profiler for at oprette [forbindelse til VPN-servere i Intune.](https://docs.microsoft.com/intune/vpn-settings-configure)  

**IOS On-Demand VPN udløses ikke, når et konfigureret domæne tilgås**

Hvis du vil teste automatiske VPN-indstillinger, skal du angive følgende værdier:

Jeg vil gøre følgende: Evaluere hvert **forsøg på at oprette forbindelse** 

Vælg, om du vil oprette forbindelse: **Forbind, hvis det er nødvendigt**

Når brugere får adgang til disse domæner:  *måldomænenavn*

Hvis ovenstående konfiguration ikke lykkes, skal du tilføje følgende element:

Når denne URL-adresse ikke er tilgængelig, skal du gennemtvinge tilslutning af VPN: **BADURL**