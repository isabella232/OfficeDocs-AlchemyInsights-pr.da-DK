---
title: Adressering af Teams-logonfejl AADSTS9000411
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
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821981"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Adressering af Teams-logonfejl AADSTS9000411

Når du logger på Microsoft Teams, modtager du muligvis fejlen: Vi beklager, men vi har problemer med at logge dig på **AADSTS9000411: Anmodningen er ikke formateret korrekt. Parameteren "login_hint" duplikeres.**

For at løse dette problem skal du sørge for, at dine Microsoft Teams-klienter opdateres. Du kan finde flere oplysninger om opdatering af din klient i [Opdater Microsoft Teams.](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)

Hvis du af en eller anden grund ikke kan opdatere din klient, rydder du de fleste cachelagrede data ved at logge af klienten. Men hvis du stadig har problemer efter logoff/logon, skal du afslutte Teams og rydde din klientcache ved at gøre følgende:
1. Luk Microsoft Teams.
2. Gå til: %appdata%\microsoft\teams, og slet alle filerne.
3. Genåå Microsoft Teams.
