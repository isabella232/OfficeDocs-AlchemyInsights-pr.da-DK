---
title: Wi-Fi-profiler i Intune
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
ms.openlocfilehash: afc8142a635b8a9d715eb4325b570be20ad26645
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696255"
---
# <a name="intune-wi-fi-profiles"></a>Wi-Fi-profiler i Intune

Vellykket implementering af Wi-Fi-forbindelse til MDM-klienter afhænger af en korrekt installeret profil, der afspejler kravene til virksomhedens Wi-Fi-infrastruktur. Hvis du vil gennemgå de relevante indstillinger for de klientplatforme, du undersøger, skal du se: 

[Tilføj Wi-Fi-indstillinger for enheder, der kører Android i Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android)

[Tilføj Wi-Fi-indstillinger for Android Enterprise-dedikerede og fuldt administrerede enheder i Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[Tilføj Wi-Fi-indstillinger for iOS-og iPadOS-enheder i Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[Tilføje Wi-Fi-indstillinger for Windows 10 og nyere enheder i Intune](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[Importere Wi-Fi-indstillinger for Windows-enheder i Intune](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**Almindelige problemer**

**Jeg installerer en Wi-Fi-profil, der er afhængig af et installeret certifikat, der er angivet i Wi-Fi-profilen. Men konfigurationsprofilerne viser en fejlstatus.**

Kontrollér, at din enhed har modtaget certifikatet.

1. Gå til **alle enheder** i Intune, og vælg enheds > **enhedskonfiguration**.

2. Kontrollér, at alle de forventede profiler er angivet og i en vellykket tilstand.

3. Hvis du har en Android-profil, skal du sørge for, at de er installeret på Android-enheder, hvis du har mellemliggende certifikater i certifikatkæden.

    Hvis du vil kontrollere certifikatstatus, skal du gå til **enheds konfigurations**  >  **profiler**  >  **Android**-  >  **Egenskaber for**  >  **certifikater, der er tillid til**.

Hvis du fortsat får vist fejlene, skal du gennemgå procedurerne og afsnittet om fejlfinding. Du kan finde flere oplysninger under [Oversigt over fejlfinding af SCEP-certifikat profiler med Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).

**Jeg har installeret en Wi-Fi-profil til en enhed. Intune viser, at det lykkedes, men enheden opretter ikke forbindelse til Wi-Fi.**

En status for succes betyder, at Intune har installeret profilen som konfigureret. Disse konfigurationer stemmer dog muligvis ikke overens med dit netværks-og/eller godkendelseskrav. Hvis du vil have mere at vide om den forsøgte forbindelse, skal du gennemgå loggene i infrastrukturen og godkendelsestjenesten (på Wi-Fi Access Point-controlleren og NPS/RADIUS-serveren). Det kan være nødvendigt at arbejde med dit netværksinfrastruktur team eller en Wi-Fi-tredjepartsleverandør for at indsamle og gennemse loggene.