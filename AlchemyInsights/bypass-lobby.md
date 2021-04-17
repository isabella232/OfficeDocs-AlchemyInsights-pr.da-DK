---
title: Gå uden om lobbyen
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
- "2673"
- "9000740"
ms.openlocfilehash: bcb40c6f15e957c0a59911322c3b28f03cd562c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820028"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Styr indstillinger for lobbyen og deltagelsesniveau i Teams

Hvis du vil tillade, at alle, herunder opkaldsbrugere, eksterne og anonyme brugere, kan springe lobbyen **over,** skal du bruge PowerShell til at udføre denne opgave. Her er et eksempel på ændring af organisationens globale mødepolitik.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Denne cmdlet kræver i øjeblikket brug af Skype for Business PowerShell-modulet. Du kan konfigurere den til at bruge denne cmdlet ved at se [Administration af politikker via PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)

Når du har konfigureret en politik, skal du anvende den til brugere. Hvis du har ændret politikken Global, gælder den automatisk for brugere. Ved enhver ændring af politikken skal du vente i mindst **4 timer op til 24** timer, før politikkerne træder i kraft. 

Sørg for at gennemgå dokumentationen nedenfor, før du foretager disse ændringer for at forstå præcis, hvad det giver mulighed for.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Forstå politikkontrolelementer for teams-mødelobbyen

Disse indstillinger styrer, hvilke mødedeltagere der venter i lobbyen, før de bliver optaget til mødet, og det deltagelsesniveau, de har tilladelse til i et møde. Du kan bruge PowerShell til at opdatere politikindstillinger for møder, der endnu ikke er blevet implementeret (mærket "kommer snart") i Teams Administration. Se nedenfor for at få et eksempel på en PowerShell-cmdlet, der giver alle brugere mulighed for at springe lobbyen over.

- [Automatisk adgang for personer](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) er en politik, der styrer, om personer deltager i et møde direkte, eller om de skal vente i lobbyen, indtil de får adgang af en godkendt bruger.

- [Tillad anonyme](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) personer at starte et møde er en politik pr. arrangør, der styrer, om anonyme personer, herunder B2B og brugere i organisationsnetværket, kan deltage i brugerens møde uden en godkendt bruger fra organisationens fremmøde.

- [Tillad opkaldsbrugere](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) at springe lobbyen **over**(Kommer snart) er en politik pr. arrangør, der styrer, om personer, der ringer ind via telefon, deltager i mødet direkte eller venter i lobbyen, uanset indstillingen Tillad automatisk adgang til **personer.**

- Tillad, at arrangører tilsidesætter indstillinger i lobbyen **(** kommer snart ) er en politik pr. arrangør, der styrer, om mødearrangøren kan tilsidesætte lobbyens indstillinger, som en administrator har angivet i Tillad automatisk adgang for personer og Tillad [opkaldsbrugere](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) at springe lobbyen over, når de planlægger et nyt møde.  

**Bemærk!** Læs [Administrer mødepolitikker i Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for at få en komplet oversigt over mødepolitikker for Microsoft Teams.
