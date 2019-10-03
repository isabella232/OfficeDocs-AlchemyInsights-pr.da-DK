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
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="3f9b2-102">Styring af lobby indstillinger og deltagelsesniveau</span><span class="sxs-lookup"><span data-stu-id="3f9b2-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="3f9b2-103">Disse indstillinger styrer, hvilke mødedeltagere der venter i lobbyen, før de får adgang til mødet, og hvor stor deltagelse de er tilladt i et møde.</span><span class="sxs-lookup"><span data-stu-id="3f9b2-103">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="3f9b2-104">Du kan bruge PowerShell til at opdatere indstillinger for møde politik, der endnu ikke er implementeret (med etiketten "kommer snart") i teams Admin Center.</span><span class="sxs-lookup"><span data-stu-id="3f9b2-104">You can use Powershell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span>  <span data-ttu-id="3f9b2-105">Se nedenfor for et eksempel PowerShell cmdlet, der giver alle brugere til at omgå lobbyen.</span><span class="sxs-lookup"><span data-stu-id="3f9b2-105">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>  

- <span data-ttu-id="3f9b2-106">[Automatisk indrømme folk](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) er en per-arrangør politik, der styrer, om folk deltage i et møde direkte eller vente i lobbyen, indtil de er optaget af en godkendt bruger.</span><span class="sxs-lookup"><span data-stu-id="3f9b2-106">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="3f9b2-107">[Tillad anonyme personer at starte et møde](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) er en politik pr. arrangør, der styrer, om anonyme personer, herunder B2B-og federated brugere, kan deltage i brugerens møde uden en godkendt bruger fra den organisation, du deltager i.</span><span class="sxs-lookup"><span data-stu-id="3f9b2-107">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="3f9b2-108">[Tillad opkaldsbrugere at omgå lobbyen](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**kommer snart**) er en per-arrangør politik, der styrer, om folk, der ringer ind via telefon deltage i mødet direkte eller vente i lobbyen, uanset den **automatisk indrømme folk** indstilling.</span><span class="sxs-lookup"><span data-stu-id="3f9b2-108">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="3f9b2-109">[Tillad arrangørerne at tilsidesætte lobby indstillinger](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**kommer snart**) er en politik pr. arrangør, der styrer, om mødearrangøren kan tilsidesætte de lobby indstillinger, som en administrator har angivet i **automatisk at indrømme personer** og **tillade opkald brugere at omgå lobbyen,** når de planlægger et nyt møde.</span><span class="sxs-lookup"><span data-stu-id="3f9b2-109">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="3f9b2-110">**Bemærk:** Læs [Administrer møde politikker i teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for at få et komplet overblik over Microsoft teams-møde politikker.</span><span class="sxs-lookup"><span data-stu-id="3f9b2-110">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span> 


<span data-ttu-id="3f9b2-111">**Eksempel på PowerShell**</span><span class="sxs-lookup"><span data-stu-id="3f9b2-111">**PowerShell example**</span></span>

<span data-ttu-id="3f9b2-112">Hvis du ønsker at tillade alle, herunder eksterne eller anonyme brugere, at omgå lobbyen, kan du også bruge PowerShell til at udføre denne opgave.</span><span class="sxs-lookup"><span data-stu-id="3f9b2-112">If you'd like to allow everyone, including external or anonymous users, to bypass the lobby, you can also use PowerShell to accomplish this task.</span></span>  <span data-ttu-id="3f9b2-113">Her er et eksempel på ændring af den globale møde politik for din organisation.</span><span class="sxs-lookup"><span data-stu-id="3f9b2-113">Here's an example of modifying the global meeting policy for your organization.</span></span>   

<span data-ttu-id="3f9b2-114">(Sørg for at gennemgå dokumentationen ovenfor, før du foretager disse ændringer for at forstå præcis, hvad dette giver mulighed for.)</span><span class="sxs-lookup"><span data-stu-id="3f9b2-114">(Be sure to review the documentation above before making these changes to understand exactly what this allows.)</span></span>

<span data-ttu-id="3f9b2-115">Set-CsTeamsMeetingPolicy-identitet global-AutoAdmittedUsers "alle"-AllowPSTNUsersToBypassLobby $True</span><span class="sxs-lookup"><span data-stu-id="3f9b2-115">Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True</span></span>

<span data-ttu-id="3f9b2-116">Yderligere oplysninger finder du i [set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="3f9b2-116">For more information, see [Set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span></span>
