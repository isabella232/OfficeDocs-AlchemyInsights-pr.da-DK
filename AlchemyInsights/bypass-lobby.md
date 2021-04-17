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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="a6f20-102">Styr indstillinger for lobbyen og deltagelsesniveau i Teams</span><span class="sxs-lookup"><span data-stu-id="a6f20-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="a6f20-103">Hvis du vil tillade, at alle, herunder opkaldsbrugere, eksterne og anonyme brugere, kan springe lobbyen **over,** skal du bruge PowerShell til at udføre denne opgave.</span><span class="sxs-lookup"><span data-stu-id="a6f20-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="a6f20-104">Her er et eksempel på ændring af organisationens globale mødepolitik.</span><span class="sxs-lookup"><span data-stu-id="a6f20-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="a6f20-105">Denne cmdlet kræver i øjeblikket brug af Skype for Business PowerShell-modulet.</span><span class="sxs-lookup"><span data-stu-id="a6f20-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="a6f20-106">Du kan konfigurere den til at bruge denne cmdlet ved at se [Administration af politikker via PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)</span><span class="sxs-lookup"><span data-stu-id="a6f20-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="a6f20-107">Når du har konfigureret en politik, skal du anvende den til brugere. Hvis du har ændret politikken Global, gælder den automatisk for brugere.</span><span class="sxs-lookup"><span data-stu-id="a6f20-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="a6f20-108">Ved enhver ændring af politikken skal du vente i mindst **4 timer op til 24** timer, før politikkerne træder i kraft.</span><span class="sxs-lookup"><span data-stu-id="a6f20-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="a6f20-109">Sørg for at gennemgå dokumentationen nedenfor, før du foretager disse ændringer for at forstå præcis, hvad det giver mulighed for.</span><span class="sxs-lookup"><span data-stu-id="a6f20-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="a6f20-110">Forstå politikkontrolelementer for teams-mødelobbyen</span><span class="sxs-lookup"><span data-stu-id="a6f20-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="a6f20-111">Disse indstillinger styrer, hvilke mødedeltagere der venter i lobbyen, før de bliver optaget til mødet, og det deltagelsesniveau, de har tilladelse til i et møde.</span><span class="sxs-lookup"><span data-stu-id="a6f20-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="a6f20-112">Du kan bruge PowerShell til at opdatere politikindstillinger for møder, der endnu ikke er blevet implementeret (mærket "kommer snart") i Teams Administration.</span><span class="sxs-lookup"><span data-stu-id="a6f20-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="a6f20-113">Se nedenfor for at få et eksempel på en PowerShell-cmdlet, der giver alle brugere mulighed for at springe lobbyen over.</span><span class="sxs-lookup"><span data-stu-id="a6f20-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="a6f20-114">[Automatisk adgang for personer](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) er en politik, der styrer, om personer deltager i et møde direkte, eller om de skal vente i lobbyen, indtil de får adgang af en godkendt bruger.</span><span class="sxs-lookup"><span data-stu-id="a6f20-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="a6f20-115">[Tillad anonyme](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) personer at starte et møde er en politik pr. arrangør, der styrer, om anonyme personer, herunder B2B og brugere i organisationsnetværket, kan deltage i brugerens møde uden en godkendt bruger fra organisationens fremmøde.</span><span class="sxs-lookup"><span data-stu-id="a6f20-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="a6f20-116">[Tillad opkaldsbrugere](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) at springe lobbyen **over**(Kommer snart) er en politik pr. arrangør, der styrer, om personer, der ringer ind via telefon, deltager i mødet direkte eller venter i lobbyen, uanset indstillingen Tillad automatisk adgang til **personer.**</span><span class="sxs-lookup"><span data-stu-id="a6f20-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="a6f20-117">Tillad, at arrangører tilsidesætter indstillinger i lobbyen **(** kommer snart ) er en politik pr. arrangør, der styrer, om mødearrangøren kan tilsidesætte lobbyens indstillinger, som en administrator har angivet i Tillad automatisk adgang for personer og Tillad [opkaldsbrugere](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) at springe lobbyen over, når de planlægger et nyt møde.  </span><span class="sxs-lookup"><span data-stu-id="a6f20-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="a6f20-118">**Bemærk!** Læs [Administrer mødepolitikker i Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for at få en komplet oversigt over mødepolitikker for Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="a6f20-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
