---
title: Logonfejl under adressering af teams AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: b70f1320ea1dfa29e6fa489bd02acfcd1d92971b
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357399"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Logonfejl under adressering af teams AADSTS9000411

Når du logger på Microsoft Teams, får du muligvis vist fejlen: **Beklager, men vi har problemer med at logge dig på AADSTS9000411: Anmodningen er ikke formateret korrekt. Parameteren "login_hint" duplikeres.**

Du kan løse dette problem ved at sikre dig, at dine Microsoft Teams-klienter er opdaterede. Yderligere oplysninger om opdatering af klienten finder du i [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

Hvis du af en eller anden grund ikke kan opdatere klienten, rydder det de fleste cachelagrede data, hvis du logger af klienten. Men hvis du stadig har problemer efter logoff/logon, skal du afslutte Teams og rydde din klientcache ved at gøre følgende:
1. Luk Microsoft Teams.
2. Gå til: %appdata%\microsoft\teams, og slet alle filerne.
3. Åbn Microsoft Teams igen.
