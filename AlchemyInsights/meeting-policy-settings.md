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
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825437"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Administrer mødepolitikker i Microsoft Teams

**Bemærk! Det kan tage op til 24 timer, før politikændringer træder i kraft for brugerne.** Du kan muligvis ikke foretage ændringer i nyligt oprettede politikker med det samme; vent 4 timer, og forsøg at ændre en nyoprettet politik igen.

Mødepolitikker bruges til at styre de funktioner, der er tilgængelige for mødedeltagere til møder, der planlægges af brugerne i organisationen. Nogle funktioner i mødepolitikker er muligvis ikke blevet implementeret i Teams Administration endnu (disse er mærket "kommer snart" i dokumentationen). I dette tilfælde, eller hvis du får en fejl som "Vi kan ikke opdatere politikken lige nu, men prøv det igen senere" i Microsoft Teams Administration, anbefaler vi, at du bruger PowerShell til at oprette eller redigere mødepolitikker for Teams. 

Du kan finde flere oplysninger om mødepolitikker i følgende ressourcer:

- Hvis du vil have mere at vide om at oprette politikker, foretage ændringer og tildele brugere til politikken, skal [du se Administrer mødepolitikker i Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Hvis du vil foretage ændringer i politikken ved hjælp af PowerShell-cmdlet'er, skal du [se Oversigt over Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Du skal bruge [Skype for Business PowerShell-modulet til](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) teams mødepolitikker. 
    - Gennemse dokumentationen [til *-CsTeamsMeetingPolicy-cmdlet'er](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for at få flere oplysninger.

