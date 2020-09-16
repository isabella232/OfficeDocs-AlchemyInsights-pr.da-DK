---
title: AADSTS9000411 for teams-logon fejl
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 8ca3793b8cd12b7ad2510ca0b3be58c32a61c14c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47687032"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>AADSTS9000411 for teams-logon fejl

Når du logger på Microsoft teams, får du muligvis fejlen: **vi beklager, men vi har problemer med at logge på AADSTS9000411: anmodningen er ikke formateret korrekt. Parameteren "login_hint" er duplikeret.**

For at løse dette problem skal du kontrollere, at dine Microsoft teams-klienter er opdateret. Du kan finde flere oplysninger om opdatering af din klient i [opdatere Microsoft teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

Hvis du ikke kan opdatere din klient af en eller anden grund, kan du logge af klienten for at rydde de fleste cachelagrede data. Men hvis du stadig har problemer efter logoff/logon, skal du afslutte teams og rydde din klientcache ved at gøre følgende:
1. Luk Microsoft teams.
2. Gå til:%AppData%\microsoft\teams og slet alle filerne.
3. Åbn Microsoft teams igen.
