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
ms.openlocfilehash: 6632bb0c09c7ce99f14cd55582025b37a846369d
ms.sourcegitcommit: ee719f011f766fc20d23e935e98d7e33c326183b
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/24/2019
ms.locfileid: "37654250"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="adbe4-102">Styring af lobby indstillinger og deltagelsesniveau</span><span class="sxs-lookup"><span data-stu-id="adbe4-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="adbe4-103">Hvis du vil tillade alle, herunder opkalds-, eksterne og anonyme brugere at omgå lobbyen, kan du bruge PowerShell til at gøre det.</span><span class="sxs-lookup"><span data-stu-id="adbe4-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users to bypass the lobby, you can use PowerShell to do it.</span></span> <span data-ttu-id="adbe4-104">Her er et eksempel på ændring af den globale møde politik for din organisation:</span><span class="sxs-lookup"><span data-stu-id="adbe4-104">Here's an example of modifying the global meeting policy for your organization:</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="adbe4-105">Denne cmdlet kræver i øjeblikket brug af Skype for Business PowerShell-modulet.</span><span class="sxs-lookup"><span data-stu-id="adbe4-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="adbe4-106">For at få setup til at bruge denne cmdlet, Tjek [Administrer politikker via PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="adbe4-106">To get setup to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="adbe4-107">Du kan oprette en ny politik, som du derefter skal anvende den på brugere.</span><span class="sxs-lookup"><span data-stu-id="adbe4-107">You can set up a new policy, which you'll then need to apply it to users.</span></span> <span data-ttu-id="adbe4-108">Hvis du ændrer den globale politik, gælder den automatisk for brugerne.</span><span class="sxs-lookup"><span data-stu-id="adbe4-108">If you modify the Global policy it'll automatically apply to users.</span></span> <span data-ttu-id="adbe4-109">For enhver politikændring, du skal vente mindst 4 timer og op til 24 timer for politikkerne træder i kraft.</span><span class="sxs-lookup"><span data-stu-id="adbe4-109">For any policy change you need to wait at least 4 hours and up to 24 hours for the policies to take effect.</span></span>

<span data-ttu-id="adbe4-110">Sørg for at gennemgå dokumentationen nedenfor, før du foretager disse ændringer for at forstå præcis, hvad dette giver mulighed for.</span><span class="sxs-lookup"><span data-stu-id="adbe4-110">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>

## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="adbe4-111">Forståelse af teams møde lobby politik kontrol</span><span class="sxs-lookup"><span data-stu-id="adbe4-111">Understanding Teams meeting lobby policy controls</span></span>

- <span data-ttu-id="adbe4-112">[Automatisk indrømme folk](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) er en per-arrangør politik, der styrer, om folk deltage i et møde direkte eller vente i lobbyen, indtil de er optaget af en godkendt bruger.</span><span class="sxs-lookup"><span data-stu-id="adbe4-112">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="adbe4-113">[Tillad anonyme personer at starte et møde](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) er en politik pr. arrangør, der styrer, om anonyme personer, herunder B2B-og federated brugere, kan deltage i brugerens møde uden en godkendt bruger fra den organisation, du deltager i.</span><span class="sxs-lookup"><span data-stu-id="adbe4-113">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="adbe4-114">[Tillad opkaldsbrugere at omgå lobbyen](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**kommer snart**) er en per-arrangør politik, der styrer, om folk, der ringer ind via telefon deltage i mødet direkte eller vente i lobbyen, uanset den **automatisk indrømme folk** indstilling.</span><span class="sxs-lookup"><span data-stu-id="adbe4-114">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="adbe4-115">[Tillad arrangørerne at tilsidesætte lobby indstillinger](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**kommer snart**) er en politik pr. arrangør, der styrer, om mødearrangøren kan tilsidesætte de lobby indstillinger, som en administrator har angivet i **automatisk at indrømme personer** og **tillade opkald brugere at omgå lobbyen,** når de planlægger et nyt møde.</span><span class="sxs-lookup"><span data-stu-id="adbe4-115">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="adbe4-116">**Bemærk:** Læs [Administrer møde politikker i teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for at få et komplet overblik over Microsoft teams-møde politikker.</span><span class="sxs-lookup"><span data-stu-id="adbe4-116">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
