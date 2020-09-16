---
title: Brug af mail profiler med Intune
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
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653282"
---
# <a name="using-email-profiles-with-intune"></a>Brug af mail profiler med Intune

Intune kan bruges til at oprette og installere mail profiler til den indbyggede mailklient på flere enheder.

Hvis du vil have oplysninger om nogle af de begrænsninger, der er knyttet til mail profiler, herunder hvordan tilstedeværelsen af eksisterende profiler håndteres, og hvordan du fjerner mail profiler, skal du se [tilføje mailindstillinger til enheder ved hjælp af Intune](https://docs.microsoft.com/intune/email-settings-configure).

Du kan finde flere oplysninger om, hvordan du opretter mail profiler for hver enhedsplatform, i:

[Indstillinger for Android-enhed for at konfigurere mail, godkendelse og synkronisering i Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Tilføje mailindstillinger for iOS-og iPadOS-enheder i Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Indstillinger for mailprofil i Microsoft Intune til enheder, der kører Windows Phone 8,1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Indstillinger for mailprofil for enheder, der kører Windows 10 i Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Almindeligt synkroniserings problem**

**En KNOX på Android-mailprofil forhindrer, at brugerkontakter, kalender og opgaver synkroniseres til bruger enheder.**

Funktionen KNOX på Android KNOX-mailprofil giver administratoren mulighed for at bestemme, hvilke indholdstyper der skal synkroniseres til enheden, ved at indstille hver til at være aktiveret.

Hvis indstillingen for en af indholdstyperne er angivet til **ikke konfigureret** (standard), synkroniseres den pågældende indholdstype ikke automatisk. En bruger kan aktivere den indholdstype, de vil have manuelt, på enheden, men konfigurationen overskrives med Intune-politikindstillingen, og synkroniseringen stopper for den pågældende indholdstype.

