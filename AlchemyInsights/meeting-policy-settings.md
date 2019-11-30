---
title: Indstillinger for møde politik
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: b5599c9974eb1c112835a9f42e4ebdc926071ea2
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627568"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Administrer møde politikker i Microsoft teams

Møde politikker bruges til at styre de funktioner, der er tilgængelige for mødedeltagere til møder, der er planlagt af brugere i organisationen. Nogle funktioner i møde politikker er muligvis ikke implementeret i teams administration endnu (disse er mærket "kommer snart" i dokumentationen). I dette tilfælde, eller hvis du får en fejl som "vi kan ikke opdatere politikken lige nu, men prøv igen senere" i Microsoft teams administration, anbefaler vi, at du bruger PowerShell til at oprette eller redigere teams-møde politikker. 

Du finder flere oplysninger om møde politikker i følgende ressourcer:

- Du kan få mere at vide om at oprette politikker, foretage ændringer og tildele brugere til politikken under [administrere møde politikker i teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Hvis du vil foretage politikændringer ved hjælp af PowerShell-cmdlets, skal du se [Oversigt i teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - Du skal bruge [Skype for Business PowerShell-modulet](https://www.microsoft.com/download/details.aspx?id=39366) til teams-møde politikker. 
    - Se [dokumentationen til cmdlet'er *-csteamsmeetingpolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for at fÃ ¥ flere oplysninger.

**Bemærk:** Det kan tage op til 24 timer, at politikændringer træder i kraft for brugerne. Du vil muligvis ikke kunne foretage ændringer af nyoprettede politikker med det samme. Vent 4 timer, og forsøg at ændre en nyoprettet politik igen. Hvis du stadig har problemer, kan du prøve PowerShell.  