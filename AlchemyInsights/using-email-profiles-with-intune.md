---
title: Brug af mailprofiler med Intune
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
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554842"
---
# <a name="using-email-profiles-with-intune"></a>Brug af mailprofiler med Intune

Intune kan bruges til at oprette og installere e-mail-profiler for den oprindelige (indbyggede) e-mail-klient på flere enhedsplatforme.

Du kan finde oplysninger om nogle af de begrænsninger, der er knyttet til mailprofiler, herunder hvordan tilstedeværelsen af eksisterende profiler håndteres, og hvordan du fjerner mailprofiler, under [Føje mailindstillinger til enheder, der bruger Intune](https://docs.microsoft.com/intune/email-settings-configure).

Du kan finde flere oplysninger om, hvordan du opretter mailprofiler for hver enhedsplatform, under:

[Indstillinger for Android-enhed til konfiguration af mail, godkendelse og synkronisering i Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Tilføje e-mail-indstillinger for iOS- og iPadOS-enheder i Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Indstillinger for mailprofil i Microsoft Intune for enheder, der kører Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Indstillinger for mailprofil for enheder, der kører Windows 10 i Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Almindeligt synkroniseringsproblem**

**En KNOX på Android-mailprofil forhindrer brugerkontakter, kalender og opgaver i at blive synkroniseret med brugerenheder.**

KNOX på Android KNOX e-mail profil giver admin mulighed for at beslutte, hvilke indholdstyper er sync'd til enheden ved at indstille hver til aktiveret.

Hvis indstillingen for en af indholdstyperne er angivet til **Ikke konfigureret** (standard), synkroniseres denne indholdstype ikke automatisk. En bruger kan aktivere den ønskede indholdstype direkte på enheden manuelt, men denne konfiguration overskrives af politikindstillingen Intune, og synkroniseringsstoppet for den pågældende indholdstype.

