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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="d2501-102">Styr lobby indstillinger og niveau for deltagelse i teams</span><span class="sxs-lookup"><span data-stu-id="d2501-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="d2501-103">Hvis du vil tillade alle, herunder opkalds-, eksterne og anonyme brugere, at **omgå lobbyen**, skal du bruge PowerShell til at udføre denne opgave.</span><span class="sxs-lookup"><span data-stu-id="d2501-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="d2501-104">Her er et eksempel på ændring af den globale møde politik for din organisation.</span><span class="sxs-lookup"><span data-stu-id="d2501-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="d2501-105">Denne cmdlet kræver i øjeblikket brug af Skype for Business PowerShell-modulet.</span><span class="sxs-lookup"><span data-stu-id="d2501-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="d2501-106">For at få sat op til at bruge denne cmdlet, Tjek [administrere politikker via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="d2501-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="d2501-107">Når du har oprettet en politik, skal du anvende den på brugere. eller, hvis du har ændret den globale politik, vil den automatisk gælde for brugere.</span><span class="sxs-lookup"><span data-stu-id="d2501-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="d2501-108">For enhver politikændring, skal du vente mindst **4 timer op til 24 timer** for politikkerne træder i kraft.</span><span class="sxs-lookup"><span data-stu-id="d2501-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="d2501-109">Sørg for at gennemgå dokumentationen nedenfor, før du foretager disse ændringer for at forstå præcis, hvad dette giver mulighed for.</span><span class="sxs-lookup"><span data-stu-id="d2501-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="d2501-110">Forståelse af teams møde lobby politik kontrol</span><span class="sxs-lookup"><span data-stu-id="d2501-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="d2501-111">Disse indstillinger styrer, hvilke mødedeltagere der venter i lobbyen, før de får adgang til mødet, og hvor stor deltagelse de er tilladt i et møde.</span><span class="sxs-lookup"><span data-stu-id="d2501-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="d2501-112">Du kan bruge PowerShell til at opdatere indstillinger for møde politik, der endnu ikke er implementeret (med etiketten "kommer snart") i teams Admin Center.</span><span class="sxs-lookup"><span data-stu-id="d2501-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="d2501-113">Se nedenfor for et eksempel PowerShell cmdlet, der giver alle brugere til at omgå lobbyen.</span><span class="sxs-lookup"><span data-stu-id="d2501-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="d2501-114">[Automatisk indrømme folk](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) er en per-arrangør politik, der styrer, om folk deltage i et møde direkte eller vente i lobbyen, indtil de er optaget af en godkendt bruger.</span><span class="sxs-lookup"><span data-stu-id="d2501-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="d2501-115">[Tillad anonyme personer at starte et møde](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) er en politik pr. arrangør, der styrer, om anonyme personer, herunder B2B-og federated brugere, kan deltage i brugerens møde uden en godkendt bruger fra den organisation, du deltager i.</span><span class="sxs-lookup"><span data-stu-id="d2501-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="d2501-116">[Tillad opkaldsbrugere at omgå lobbyen](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**kommer snart**) er en per-arrangør politik, der styrer, om folk, der ringer ind via telefon deltage i mødet direkte eller vente i lobbyen, uanset den **automatisk indrømme folk** indstilling.</span><span class="sxs-lookup"><span data-stu-id="d2501-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="d2501-117">[Tillad arrangørerne at tilsidesætte lobby indstillinger](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**kommer snart**) er en politik pr. arrangør, der styrer, om mødearrangøren kan tilsidesætte de lobby indstillinger, som en administrator har angivet i **automatisk at indrømme personer** og **tillade opkaldsbrugere at omgå lobbyen** , når de planlægger et nyt møde.</span><span class="sxs-lookup"><span data-stu-id="d2501-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="d2501-118">**Bemærk:** Læs [Administrer møde politikker i teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for at få et komplet overblik over Microsoft teams-møde politikker.</span><span class="sxs-lookup"><span data-stu-id="d2501-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
