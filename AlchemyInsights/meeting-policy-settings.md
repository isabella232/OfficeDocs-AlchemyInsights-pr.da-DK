---
title: Indstillinger for mødepolitik
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 06395bcc1a631adeaa8abb5ad63b971639f226c19e48203078ba1097d43a50f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925159"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Administrer mødepolitikker i Microsoft Teams

**Bemærk! Det kan tage op til 24 timer, før politikændringer træder i kraft for brugerne.** Du kan muligvis ikke foretage ændringer i nyligt oprettede politikker med det samme; vent 4 timer, og forsøg at ændre en nyoprettet politik igen.

Mødepolitikker bruges til at styre de funktioner, der er tilgængelige for mødedeltagere til møder, der planlægges af brugerne i organisationen. Nogle funktioner i mødepolitikker er muligvis ikke blevet implementeret i Teams Administration endnu (disse er mærket "kommer snart" i dokumentationen). I dette tilfælde, eller hvis du får en fejl som "Vi kan ikke opdatere politikken lige nu, men prøv den igen senere" i Microsoft Teams Administration, anbefaler vi, at du bruger PowerShell til at oprette eller redigere Teams-mødepolitikker. 

Du kan finde flere oplysninger om mødepolitikker i følgende ressourcer:

- Du kan få mere at vide om at oprette politikker, foretage ændringer og tildele brugere til politikken under Administrere [mødepolitikker i Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Hvis du vil foretage ændringer i politikken ved hjælp af PowerShell-cmdlet'er, [skal Teams oversigt over PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - Du skal bruge Skype for Business [PowerShell-modulet til](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) Teams mødepolitikker. 
    - Gennemse dokumentationen [til *-CsTeamsMeetingPolicy-cmdlet'er](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for at få flere oplysninger.

