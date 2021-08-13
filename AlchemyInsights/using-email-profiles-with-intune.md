---
title: Brug af mailprofiler med Intune
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
- "1559"
- "9000076"
ms.openlocfilehash: b1653b73e7296e7eed411ae73c19342a1187b2eb7e287cff4339ea0ca32d75c1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919417"
---
# <a name="using-email-profiles-with-intune"></a>Brug af mailprofiler med Intune

Intune kan bruges til at oprette og installere mailprofiler for den oprindelige (indbyggede) mailklient på flere enhedsplatforme.

Hvis du vil have oplysninger om nogle af de begrænsninger, der er knyttet til mailprofiler, herunder hvordan tilstedeværelsen af eksisterende profiler håndteres, og hvordan du fjerner mailprofiler, skal du se Føj mailindstillinger til enheder ved hjælp af [Intune](https://docs.microsoft.com/intune/email-settings-configure).

Du kan finde flere oplysninger om, hvordan du opretter mailprofiler for hver enhedsplatform, under:

[Indstillinger for Android-enheder til konfiguration af mail, godkendelse og synkronisering i Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Tilføj mailindstillinger for iOS- og iPadOS-enheder i Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Indstillinger for mailprofil i Microsoft Intune for enheder, der Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Indstillinger for mailprofil for enheder, der Windows 10 i Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Almindeligt synkroniseringsproblem**

**En KNOX på Android-mailprofil forhindrer brugerkontakter, kalender og opgaver i at blive synkroniseret til brugerenheder.**

KNOX på Android KNOX-mailprofilen giver administratoren mulighed for at beslutte, hvilke indholdstyper der synkroniseres med enheden, ved at indstille hver af dem til aktiveret.

Hvis indstillingen for nogen af indholdstyperne er angivet til Ikke konfigureret **(standard),** synkroniseres den pågældende indholdstype ikke automatisk. En bruger kan aktivere den ønskede indholdstype direkte på enheden manuelt, men denne konfiguration overskrives af intune-politikindstillingen, og synkroniseringen stopper for den pågældende indholdstype.

