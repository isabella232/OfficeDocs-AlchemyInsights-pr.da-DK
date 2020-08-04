---
title: VPN-relaterede problemer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554838"
---
# <a name="vpn-related-issues"></a>VPN-relaterede problemer

En vellykket implementering af VPN-forbindelse til MDM-klienter afhænger af en installeret profil, der korrekt afspejler kravene i VPN-infrastrukturen. Du kan se de relevante indstillinger for de klientplatforme, du undersøger, på: 

[Indstillinger for Windows 10 og Windows Holographic device for at tilføje VPN-forbindelser ved hjælp af Intune](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[Tilføje VPN-indstillinger på iOS- og iPadOS-enheder i Microsoft Intune](https://docs.microsoft.com/intune/vpn-settings-ios)  
[Indstillinger for Android-enhed til konfiguration af VPN i Intune](https://docs.microsoft.com/intune/vpn-settings-android)  
[Tilføje VPN-indstillinger på macOS-enheder i Microsoft Intune](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

Hvis din VPN-profil bruger certifikatbaseret godkendelse, skal du sørge for, at de rodcertifikat- og klientgodkendelsescertifikatprofiler, der er knyttet til VPN-profilen, er installeret korrekt.

**Almindelige problemer**

**Jeg har indsat en VPN-profil på en enhed. Intune viser, at det lykkedes, men enheden opretter ikke forbindelse til VPN.**

En vellykket status betyder, at Intune har installeret profilen som konfigureret. Disse konfigurationer svarer dog muligvis ikke til dine netværks- og/eller godkendelseskrav. Gennemse logfiler i infrastruktur- og godkendelsestjenesten (på VPN-serveren og NPS/Radius-serveren) for at få flere oplysninger om den forsøgte forbindelse. Du skal muligvis samarbejde med dit netværksinfrastrukturteam eller tredjeparts VPN-leverandøren for at indsamle og gennemse logfiler.

**Når jeg konfigurerer en brugerdefineret VPN til iOS, bliver VPN-funktionen pr. app ikke gjort tilgængelig.**

Vpn per-app til iOS-enheder i Intune er i øjeblikket tilgængelig for en bestemt liste over udbydere og partnere, som også skal opfylde certifikatforudsætningerne, før du konfigurerer en VPN pr. app. Du kan finde flere oplysninger [under Konfigurere VPN (Virtual Private Network) pr. app (VPN) til iOS/iPadOS-enheder i Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app). 

Du kan finde flere oplysninger om alle VPN-forbindelsestyper i Intune under [Oprette VPN-profiler for at oprette forbindelse til VPN-servere i Intune](https://docs.microsoft.com/intune/vpn-settings-configure).  

**iOS On-Demand VPN udløses ikke, når der opnås adgang til et konfigureret domæne**

Hvis du vil teste automatiske VPN-indstillinger, skal du angive følgende værdier:

Jeg vil gøre følgende: **Vurder hvert forsøg på at oprette forbindelse** 

Vælg, om der skal oprettes forbindelse: **Opret forbindelse, hvis det er nødvendigt**

Når brugere får adgang til disse domæner: **target** *måldomænenavn*

Hvis ovenstående konfiguration ikke lykkes, skal du tilføje følgende element:

Når denne URL-adresse ikke kan nås, skal du tvinge VPN: **BADURL**