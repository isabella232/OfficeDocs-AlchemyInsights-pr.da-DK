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
ms.openlocfilehash: de665ca6defcd0d00d227435473e5a4ccf61bc82
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376585"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Styring af lobby indstillinger og deltagelsesniveau

Disse indstillinger styrer, hvilke mødedeltagere der venter i lobbyen, før de får adgang til mødet, og hvor stor deltagelse de er tilladt i et møde. Du kan bruge PowerShell til at opdatere indstillinger for møde politik, der endnu ikke er implementeret (med etiketten "kommer snart") i teams Admin Center.  Se nedenfor for et eksempel PowerShell cmdlet, der giver alle brugere til at omgå lobbyen.  

- [Automatisk indrømme folk](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) er en per-arrangør politik, der styrer, om folk deltage i et møde direkte eller vente i lobbyen, indtil de er optaget af en godkendt bruger.

- [Tillad anonyme personer at starte et møde](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) er en politik pr. arrangør, der styrer, om anonyme personer, herunder B2B-og federated brugere, kan deltage i brugerens møde uden en godkendt bruger fra den organisation, du deltager i.

- [Tillad opkaldsbrugere at omgå lobbyen](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**kommer snart**) er en per-arrangør politik, der styrer, om folk, der ringer ind via telefon deltage i mødet direkte eller vente i lobbyen, uanset den **automatisk indrømme folk** indstilling.

- [Tillad arrangørerne at tilsidesætte lobby indstillinger](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**kommer snart**) er en politik pr. arrangør, der styrer, om mødearrangøren kan tilsidesætte de lobby indstillinger, som en administrator har angivet i **automatisk at indrømme personer** og **tillade opkald brugere at omgå lobbyen,** når de planlægger et nyt møde.

**Bemærk:** Læs [Administrer møde politikker i teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for at få et komplet overblik over Microsoft teams-møde politikker. 


**Eksempel på PowerShell**

Hvis du ønsker at tillade alle, herunder eksterne eller anonyme brugere, at omgå lobbyen, kan du også bruge PowerShell til at udføre denne opgave.  Her er et eksempel på ændring af den globale møde politik for din organisation.   

(Sørg for at gennemgå dokumentationen ovenfor, før du foretager disse ændringer for at forstå præcis, hvad dette giver mulighed for.)

Set-CsTeamsMeetingPolicy-identitet global-AutoAdmittedUsers "alle"-AllowPSTNUsersToBypassLobby $True

Yderligere oplysninger finder du i [set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).
