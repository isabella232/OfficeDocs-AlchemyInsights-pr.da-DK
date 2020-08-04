---
title: Intune Wi-Fi-profiler
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
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/29/2020
ms.locfileid: "46554858"
---
# <a name="intune-wi-fi-profiles"></a>Intune Wi-Fi-profiler

En vellykket implementering af Wi-Fi-forbindelse til MDM-klienter afhænger af en korrekt installeret profil, der afspejler kravene i virksomhedens Wi-Fi-infrastruktur. Hvis du vil gennemse de relevante indstillinger for de klientplatforme, du undersøger, skal du se: 

[Tilføje Wi-Fi-indstillinger for enheder, der kører Android i Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android)

[Tilføj Wi-Fi-indstillinger til Android Enterprise-dedikerede og fuldt administrerede enheder i Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[Tilføje Wi-Fi-indstillinger til iOS- og iPadOS-enheder i Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[Tilføje Wi-Fi-indstillinger for Windows 10 og nyere enheder i Intune](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[Importere Wi-Fi-indstillinger for Windows-enheder i Intune](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**Almindelige problemer**

**Jeg installerer en Wi-Fi-profil, der er afhængig af et installeret certifikat, der er angivet i Wi-Fi-profilen. Konfigurationsprofilerne viser dog en fejlstatus.**

Kontroller, at enheden har modtaget certifikatet.

1. Gå til Alle enheder i **Intune, og** vælg > **enhedskonfiguration .**

2. Kontroller, at alle forventede profiler er angivet og i en vellykket tilstand.

3. Hvis du har mellemliggende certifikater i din certifikatkæde for en Android-profil, skal du sørge for, at de er installeret på Android-enheder.

    Hvis du vil kontrollere certifikatstatus, skal du gå til **Android**Intermediate CA Properties Trusted Certificate for  >  **enhedskonfigurationsprofiler.**  >  **Android intermediate CA**  >  **Properties**  >  **Trusted Certificate**

Hvis du bliver ved med at se fejl, skal du gennemgå procedurerne og afsnittet fejlfinding. Du kan finde flere oplysninger [under Oversigt over fejlfinding af SCEP-certifikatprofiler med Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).

**Jeg har installeret en Wi-Fi-profil på en enhed. Intune viser, at det lykkedes, men enheden opretter ikke forbindelse til Wi-Fi.**

En vellykket status betyder, at Intune har installeret profilen som konfigureret. Disse konfigurationer svarer dog muligvis ikke til dine netværks- og/eller godkendelseskrav. Du kan få flere oplysninger om den forsøgte forbindelse ved at gennemse logfiler i infrastrukturen og godkendelsestjenesten (på Wi-Fi-adgangspunktcontrolleren og NPS/Radius-serveren). Du skal muligvis samarbejde med dit netværksinfrastrukturteam eller tredjeparts-Wi-Fi-leverandøren for at indsamle og gennemse logfiler.