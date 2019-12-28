---
title: Bypass lobby
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 311af365a94b788182bb6870bca3f67b2ad802d0
ms.sourcegitcommit: 932981641dd8e973e28dfe346bbdf9c923111b13
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/27/2019
ms.locfileid: "40889076"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Styr lobby indstillinger og niveau for deltagelse i teams

Hvis du vil tillade alle, herunder opkalds-, eksterne og anonyme brugere, at **omgå lobbyen**, skal du bruge PowerShell til at udføre denne opgave. Her er et eksempel på ændring af den globale møde politik for din organisation.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Denne cmdlet kræver i øjeblikket brug af Skype for Business PowerShell-modulet. For at få sat op til at bruge denne cmdlet, Tjek [administrere politikker via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Når du har oprettet en politik, skal du anvende den på brugere. eller, hvis du har ændret den globale politik, vil den automatisk gælde for brugere. For enhver politikændring, skal du vente mindst **4 timer op til 24 timer** for politikkerne træder i kraft. 

Sørg for at gennemgå dokumentationen nedenfor, før du foretager disse ændringer for at forstå præcis, hvad dette giver mulighed for.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Forståelse af teams møde lobby politik kontrol

Disse indstillinger styrer, hvilke mødedeltagere der venter i lobbyen, før de får adgang til mødet, og hvor stor deltagelse de er tilladt i et møde. Du kan bruge PowerShell til at opdatere indstillinger for møde politik, der endnu ikke er implementeret (med etiketten "kommer snart") i teams Admin Center. Se nedenfor for et eksempel PowerShell cmdlet, der giver alle brugere til at omgå lobbyen.

- [Automatisk indrømme folk](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) er en per-arrangør politik, der styrer, om folk deltage i et møde direkte eller vente i lobbyen, indtil de er optaget af en godkendt bruger.

- [Tillad anonyme personer at starte et møde](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) er en politik pr. arrangør, der styrer, om anonyme personer, herunder B2B-og federated brugere, kan deltage i brugerens møde uden en godkendt bruger fra den organisation, du deltager i.

- [Tillad opkaldsbrugere at omgå lobbyen](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**kommer snart**) er en per-arrangør politik, der styrer, om folk, der ringer ind via telefon deltage i mødet direkte eller vente i lobbyen, uanset den **automatisk indrømme folk** indstilling.

- [Tillad arrangørerne at tilsidesætte lobby indstillinger](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**kommer snart**) er en politik pr. arrangør, der styrer, om mødearrangøren kan tilsidesætte de lobby indstillinger, som en administrator har angivet i **automatisk at indrømme personer** og **tillade opkaldsbrugere at omgå lobbyen** , når de planlægger et nyt møde.

**Bemærk:** Læs [Administrer møde politikker i teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for at få et komplet overblik over Microsoft teams-møde politikker.
