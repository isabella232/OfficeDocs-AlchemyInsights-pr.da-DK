---
title: Teams starter ikke
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/4/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12673"
- "9007646"
ms.openlocfilehash: a37f980e700090da8199c703216af6f04f4aca464c21870beb3e907dd7b2d491
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813344"
---
# <a name="teams-doesnt-launch"></a>Teams starter ikke

Hvis du forsøger at åbne en Microsoft Teams men den aldrig starter, kan du prøve følgende:

1. Gå til **%appdata%\Microsoft\Teams**.
1. Slet indholdet af mappen.
1. Genstart computeren, og prøv at starte Teams.

Du skal muligvis geninstallere Teams. Sådan geninstallerer du:

1. Fjern Teams ved hjælp af Kontrolpanel.
1. Gå til **%appdata%\Microsoft\Teams\Application Cache.**
1. Slet indholdet af mappen.
1. Gå til **%appdata%\Microsoft\teams\Cache.**
1. Slet indholdet af mappen.
1. Genstart computeren, og download og installér derefter Teams.

Hvis du vil køre en diagnosticering på din lejer for en bestemt bruger, der ikke kan logge på, kan du starte en ny søgning med nøgleordet **TeamsUserUnableToSignIn** og følge instruktionerne.