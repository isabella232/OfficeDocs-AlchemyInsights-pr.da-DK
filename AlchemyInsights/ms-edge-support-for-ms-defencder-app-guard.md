---
title: Microsoft Edge-understøttelse af Microsoft Defender Application Guard
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583367"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a>Microsoft Edge-understøttelse af Microsoft Defender Application Guard

Application Guard, der er udviklet til Windows 10 og Microsoft Edge, anvender en hardware isolations metode, der gør det muligt for en bruger at navigere i et websted, der ikke er tillid til, fra en isoleret, Hyper-V-aktiveret beholder, adskilt fra værtsoperativsystemet.

En virksomhedsadministrator definerer en liste over websteder, der er tillid til, Cloud-ressourcer og interne netværk. Når en bruger besøger et websted, der ikke er på listen, vil Microsoft Edge åbne webstedet i beholderen. Det betyder, at hvis webstedet nedsættes for at være skadeligt, vil værtscomputeren fortsat være beskyttet, og hackeren vil ikke komme til virksomhedens data.

Installation af udvidelser i beholderen understøttes af Microsoft Edge version 81, og den kan kontrolleres via en politik. UpdateURL-adressen, der bruges i ExtensionInstallForcelist-politikken, skal tilføjes som en neutral ressource i de politikker for netværks isolation, der bruges af Application Guard.

Du kan finde flere oplysninger i [Microsoft Edge support til Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).
