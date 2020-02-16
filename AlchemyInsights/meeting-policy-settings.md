---
title: Indstillinger for mødepolitik
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 509bd0c686830c04ed27f97372411677c0a7f4a4
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/15/2020
ms.locfileid: "42042838"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Administrere mødepolitikker i Microsoft Teams

**Bemærk: Det kan tage op til 24 timer, før politikændringer træder i kraft for brugerne.** Du kan muligvis ikke foretage ændringer i nyoprettede politikker med det samme. vente 4 timer og forsøge at ændre en nyoprettet politik igen.

Mødepolitikker bruges til at styre de funktioner, der er tilgængelige for mødedeltagere til møder, der er planlagt af brugere i organisationen. Nogle funktioner i mødepolitikker er muligvis ikke implementeret i Teams Administration endnu (disse er mærket "kommer snart" i dokumentationen). I dette tilfælde, eller hvis du får en fejl som "Vi kan ikke opdatere politikken lige nu, men prøv den igen senere" i Microsoft Teams Administration, anbefaler vi, at du bruger PowerShell til at oprette eller ændre politikker for holdmøde. 

Yderligere oplysninger om mødepolitikker finder du i følgende ressourcer:

- Hvis du vil have mere at vide om at oprette politikker, foretage ændringer og tildele brugere til politikken, skal du se [Administrere mødepolitikker i Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Hvis du vil foretage politikændringer ved hjælp af PowerShell-cmdletter, skal du se [Teams PowerShell Oversigt](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Du skal bruge [Skype for Business PowerShell-modulet](https://www.microsoft.com/download/details.aspx?id=39366) til teams mødepolitikker. 
    - Læs [dokumentationen til cmdletterne *-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for at få flere oplysninger.

