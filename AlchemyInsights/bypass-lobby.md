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
ms.openlocfilehash: 729fc5d4213acbbdf74a9d07adacb42b34170717
ms.sourcegitcommit: ffbeb72c9199ab4ebcb0f1ad443ed3e2f4950efc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/23/2019
ms.locfileid: "37637771"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Styring af lobby indstillinger og deltagelsesniveau

Hvis du vil tillade alle, herunder opkalds-, eksterne og anonyme brugere at omgå lobbyen, kan du bruge PowerShell til at gøre det. Her er et eksempel på ændring af den globale møde politik for din organisation:

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Denne cmdlet kræver i øjeblikket brug af Skype for Business PowerShell-modulet. For at få setup til at bruge denne cmdlet, tjek Administrer politikker via PowerShell.

Du kan oprette en ny politik, som du derefter skal anvende den på brugere. Hvis du ændrer den globale politik, gælder den automatisk for brugerne. For enhver politikændring, du skal vente mindst 4 timer og op til 24 timer for politikkerne træder i kraft.

Sørg for at gennemgå dokumentationen nedenfor, før du foretager disse ændringer for at forstå præcis, hvad dette giver mulighed for.

## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Forståelse af teams møde lobby politik kontrol

- [Automatisk indrømme folk](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) er en per-arrangør politik, der styrer, om folk deltage i et møde direkte eller vente i lobbyen, indtil de er optaget af en godkendt bruger.

- [Tillad anonyme personer at starte et møde](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) er en politik pr. arrangør, der styrer, om anonyme personer, herunder B2B-og federated brugere, kan deltage i brugerens møde uden en godkendt bruger fra den organisation, du deltager i.

- [Tillad opkaldsbrugere at omgå lobbyen](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**kommer snart**) er en per-arrangør politik, der styrer, om folk, der ringer ind via telefon deltage i mødet direkte eller vente i lobbyen, uanset den **automatisk indrømme folk** indstilling.

- [Tillad arrangørerne at tilsidesætte lobby indstillinger](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**kommer snart**) er en politik pr. arrangør, der styrer, om mødearrangøren kan tilsidesætte de lobby indstillinger, som en administrator har angivet i **automatisk at indrømme personer** og **tillade opkald brugere at omgå lobbyen,** når de planlægger et nyt møde.

**Bemærk:** Læs [Administrer møde politikker i teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for at få et komplet overblik over Microsoft teams-møde politikker.
