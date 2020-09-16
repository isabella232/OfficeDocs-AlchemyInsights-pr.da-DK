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
ms.openlocfilehash: 3c031725c92f5d7af7c0dd0c37ea34fecf4792c8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47726085"
---
# <a name="vpn-related-issues"></a>VPN-relaterede problemer

Vellykket implementering af VPN-forbindelse for MDM-klienter afhænger af en installeret profil, der afspejler kravene til VPN-infrastrukturen korrekt. Du kan finde relevante indstillinger for de klientplatforme, du undersøger, under: 

[Enhedsindstillinger for Windows 10 og Windows Holographic for at tilføje VPN-forbindelser ved hjælp af Intune](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[Tilføje VPN-indstillinger på iOS-og iPadOS-enheder i Microsoft Intune](https://docs.microsoft.com/intune/vpn-settings-ios)  
[Indstillinger for Android-enhed til konfiguration af VPN i Intune](https://docs.microsoft.com/intune/vpn-settings-android)  
[Tilføje VPN-indstillinger på macOS-enheder i Microsoft Intune](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

Hvis din VPN-profil brugercertifikat baseret godkendelse, skal du kontrollere, at de rodcertifikater for rodcertifikater og klientgodkendelses certifikater, der er knyttet til VPN-profilen, er blevet installeret korrekt.

**Almindelige problemer**

**Jeg har installeret en VPN-profil på en enhed. Intune viser, at det lykkedes, men enheden opretter ikke forbindelse til VPN.**

En status for succes betyder, at Intune har installeret profilen som konfigureret. Disse konfigurationer stemmer dog muligvis ikke overens med dit netværks-og/eller godkendelseskrav. Gennemse loggene i infrastrukturen og godkendelsestjenesten (på VPN-serveren og NPS/RADIUS-serveren) for at få flere oplysninger om den forsøgte forbindelse. Det kan være nødvendigt at arbejde med dit netværksinfrastruktur team eller en VPN-leverandør fra tredjepartsleverandører for at indsamle og gennemse loggene.

**Når jeg konfigurerer en brugerdefineret VPN til iOS, bliver VPN-funktionen pr. app ikke tilgængelig.**

Per-App VPN til iOS-enheder i Intune er i øjeblikket tilgængelig for en bestemt liste over udbydere og partnere, som også skal opfylde certifikatets forudsætninger, før du konfigurerer en per-appen VPN. Hvis du vil have mere at vide, skal du se [konfigurere per-app virtuelt privat netværk (VPN) til iOS/iPadOS-enheder i Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app). 

Du kan finde flere oplysninger om alle VPN-forbindelsestyper i Intune under [oprette VPN-profiler for at oprette forbindelse til VPN-servere i Intune](https://docs.microsoft.com/intune/vpn-settings-configure).  

**iOS on-demand VPN udløser ikke, når der opnås adgang til et konfigureret domæne**

Hvis du vil teste automatiske VPN-indstillinger, skal du angive følgende værdier:

Jeg vil gøre følgende: **Evaluer hvert forbindelsesforsøg** 

Vælg, om du vil oprette forbindelse: **Opret forbindelse, hvis det er nødvendigt**

Når brugere får adgang til disse domæner: **destinations** *domænenavn*

Hvis ovenstående konfiguration ikke lykkes, skal du tilføje følgende element:

Når denne URL-adresse ikke kan oprettes, skal du oprette forbindelse til VPN: **BADURL**