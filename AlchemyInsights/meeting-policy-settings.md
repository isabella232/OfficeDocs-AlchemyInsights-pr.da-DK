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
ms.openlocfilehash: dac06690b51459ca166c15a5ef0f4c7e7a6d36f0
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376580"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Administrer møde politikker i Microsoft teams

Møde politikker bruges til at styre de funktioner, der er tilgængelige for mødedeltagere til møder, der er planlagt af brugere i organisationen. Nogle funktioner i møde politikker er muligvis ikke implementeret i teams administration endnu (disse er mærket "kommer snart" i dokumentationen). I dette tilfælde, eller hvis du får en fejl som "vi kan ikke opdatere politikken lige nu, men prøv igen senere" i Microsoft teams administration, anbefaler vi, at du bruger PowerShell til at oprette eller redigere teams-møde politikker. 

Du finder flere oplysninger om møde politikker i følgende ressourcer:

- Du kan få mere at vide om at oprette politikker, foretage ændringer og tildele brugere til politikken under [administrere møde politikker i teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).

- Hvis du vil foretage politikændringer ved hjælp af PowerShell-cmdlets, skal du se [Oversigt i teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - Du skal bruge [Skype for Business PowerShell-modulet](https://www.microsoft.com/download/details.aspx?id=39366) til teams-møde politikker. 
    - Se [dokumentationen til cmdlet'er *-csteamsmeetingpolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for at fÃ ¥ flere oplysninger.

**Bemærk:** Det kan tage op til 24 timer, at politikændringer træder i kraft for brugerne. Du vil muligvis ikke kunne foretage ændringer af nyoprettede politikker med det samme. Vent 4 timer, og forsøg at ændre en nyoprettet politik igen. Hvis du stadig har problemer, kan du prøve PowerShell.  