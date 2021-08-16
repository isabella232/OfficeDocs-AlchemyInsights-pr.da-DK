---
title: Intune Wi-Fi profiler
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
- "1548"
- "9000076"
ms.openlocfilehash: 5e5258806c8a38965467a8878bc8ac922c2668f21abe3602f479dcdaff8c9b5b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028214"
---
# <a name="intune-wi-fi-profiles"></a>Intune Wi-Fi profiler

En vellykket implementering Wi-Fi forbindelse for MDM-klienter afhænger af en korrekt installeret profil, der afspejler kravene fra virksomhedens Wi-Fi infrastruktur. Hvis du vil gennemgå de relevante indstillinger for de klientplatforme, du undersøger, skal du se: 

[Tilføj Wi-Fi for enheder, der kører Android i Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android)

[Tilføj Wi-Fi indstillinger for Android Enterprise dedikerede og fuldt administrerede enheder i Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[Tilføj Wi-Fi indstillinger for iOS- og iPadOS-enheder i Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[Tilføj Wi-Fi indstillinger for Windows 10 og nyere enheder i Intune](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[Importér Wi-Fi indstillinger for Windows-enheder i Intune](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**Almindelige problemer**

**Jeg udruller en Wi-Fi, der er afhængig af et installeret certifikat, der er angivet i Wi-Fi profil. Men konfigurationsprofilerne viser en fejlstatus.**

Kontrollér, at din enhed har modtaget certifikatet.

1. I Intune skal du gå **til Alle enheder og** vælge enheden > **Enhedskonfiguration.**

2. Kontrollér, at alle forventede profiler er angivet og i en vellykket tilstand.

3. Hvis du har mellemliggende certifikater i din certifikatkæde til en Android-profil, skal du sikre dig, at de er installeret på Android-enheder.

    Hvis du vil kontrollere certifikatstatus, skal du gå til **Enhedskonfigurationsprofiler** for  >    >  **Android-mellemliggende nøglecenteregenskaber,**  >  **der er** tillid til  >  **certifikat**.

Hvis du fortsat får vist fejl, skal du gennemse procedurerne og fejlfindingssektionerne. Få mere at vide under [Oversigt over fejlfinding af SCEP-certifikatprofiler med Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).

**Jeg har installeret Wi-Fi profil på en enhed. Intune viser, at det lykkedes, men enheden opretter ikke forbindelse til Wi-Fi-forbindelsen.**

En vellykket status betyder, at Intune har installeret profilen som konfigureret. Disse konfigurationer opfylder dog muligvis ikke dine krav til netværk og/eller godkendelse. Du kan finde flere oplysninger om den forsøgte forbindelse ved at gennemse logge i infrastrukturen og autentifikationsservice (på Wi-Fi Access point controller og NPS/Radius-server). Du skal muligvis arbejde med dit netværksinfrastrukturteam eller tredjepartsudbyderen af Wi-Fi for at indsamle og gennemse logfiler.