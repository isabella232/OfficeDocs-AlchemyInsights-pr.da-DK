---
title: Tilsidesæt informations
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684944"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Kontroller informations indstillinger og niveau for deltagelse i teams

Hvis du vil tillade, at alle, herunder opkalds-, eksterne og anonyme brugere, skal kunne **omgå informations funktionen**, skal du bruge PowerShell til at udføre denne opgave. Her er et eksempel på ændring af den globale møde politik for din organisation.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Denne cmdlet kræver i øjeblikket brugen af Skype for Business PowerShell-modulet. For at få konfigureret til at bruge denne cmdlet skal du se [administration af politikker via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Når du har konfigureret en politik, skal du anvende den på brugerne. eller hvis du har ændret den globale politik, gælder den automatisk for brugere. Du skal vente mindst **4 timer op til 24 timer** , før politikkerne træder i kraft, for at du kan ændre politikken. 

Sørg for at gennemgå dokumentationen nedenfor, før du foretager disse ændringer for at forstå, hvad dette giver mulighed for.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Forstå kontrolelementer til politik for mødets informationspolitik

Disse indstillinger styrer, hvilke mødedeltagere der skal vente i informations samarbejdet, før de deltager i mødet, og det tilsvarende omfang de er tilladt i et møde. Du kan bruge PowerShell til at opdatere indstillinger for møde politik, der endnu ikke er implementeret (kaldet "kommer snart") i teams administration. Se nedenfor for at få et eksempel på en PowerShell-cmdlet, der gør det muligt for alle brugere at omgå informations funktionen.

- Giv [automatisk personer](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) en per-Organizer-politik, der styrer, om personer deltager i et møde direkte eller venter i informations funktionen, indtil de er optaget af en godkendt bruger.

- [Tillad, at anonyme personer starter et møde](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) , er en politik om arrangøren, der styrer, om anonyme personer, herunder B2B-og organisations brugere, kan deltage i brugerens møde uden en godkendt bruger fra organisationen i fremmøde.

- [Giv opkalds brugere mulighed for at omgå informations](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) udbyderen (**kommer snart**) er en politik om arrangøren, der styrer, om personer, der ringer ind via telefon, kan deltage i mødet direkte eller vente i informations funktionen, uanset om indstillingen Giv **personer automatisk** er blevet givet.

- [Tillad, at arrangører kan tilsidesætte informations indstillinger](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**kommer snart**) er en politik om arrangøren, der styrer, om mødearrangøren kan tilsidesætte de informations indstillinger, som en administrator har angivet i **automatisk give personer** **tilladelse til at undgå, at opkalds brugere** går i gang med at planlægge et nyt møde.

**Bemærk:** Læs [Administrer møde politikker i teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for at få en komplet oversigt over møde politikker i Microsoft teams.
