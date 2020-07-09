---
title: Problemet med udskriftsspooler er løst
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 53b1c9a8efa3cc978af8b602c8ed90430042186a
ms.sourcegitcommit: 4265a9e79db6c2a396aa80ec0ebd467bbaadf366
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/08/2020
ms.locfileid: "45088304"
---
# <a name="print-spooler-issue-is-resolved"></a>Problemet med udskriftsspooler er løst

Hvis enheden er blevet opdateret med Windows 10 **OS Build 19041.329**, har du muligvis observeret et problem, hvor visse printere ikke udskrives. Udskriftsspooleren kan kaste en fejl eller lukke uventet, når du forsøger at udskrive, og der kommer ingen udgang fra den berørte printer. Dette problem er løst i OS Build **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).  

**Igangværende undersøgelse**

LSASS-filen (Local Security Authority Subsystem Service)** (Isass.exe**) kan mislykkes på nogle enheder med fejlmeddelelsen "En kritisk systemproces, C:\WINDOWS\system32\Isass.exe mislykkedes med statuskoden c0000008. Maskinen skal nu genstartes".  **Microsoft arbejder på en løsning og leverer en opdatering i en kommende version.**

Du kan finde flere oplysninger i kendte problemer i [Windows 10 Version 2004](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).