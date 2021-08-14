---
title: Adressering Teams logonfejl AADSTS9000411
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 883bf48d3628702c92361a5250f0d59e1352918349b8bc6c3eae5a948b72fc57
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53953009"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Adressering Teams logonfejl AADSTS9000411

Når du logger på Microsoft Teams, modtager du muligvis fejlen: Vi beklager, men vi har problemer med at logge dig på **AADSTS9000411: Anmodningen er ikke formateret korrekt. Parameteren "login_hint" duplikeres.**

For at løse dette problem skal du sikre dig, Microsoft Teams klientklienterne er opdateret. Du kan finde flere oplysninger om opdatering af din klient [under Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

Hvis du af en eller anden grund ikke kan opdatere din klient, rydder du de fleste cachelagrede data ved at logge af klienten. Men hvis du stadig har problemer efter logoff/logon, skal du afslutte Teams og rydde klientcachen ved at gøre følgende:
1. Luk Microsoft Teams.
2. Gå til: %appdata%\microsoft\teams, og slet alle filerne.
3. Åbn Microsoft Teams.
