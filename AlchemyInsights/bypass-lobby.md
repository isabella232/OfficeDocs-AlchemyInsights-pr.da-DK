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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="0d04a-102">Kontroller informations indstillinger og niveau for deltagelse i teams</span><span class="sxs-lookup"><span data-stu-id="0d04a-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="0d04a-103">Hvis du vil tillade, at alle, herunder opkalds-, eksterne og anonyme brugere, skal kunne **omgå informations funktionen**, skal du bruge PowerShell til at udføre denne opgave.</span><span class="sxs-lookup"><span data-stu-id="0d04a-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="0d04a-104">Her er et eksempel på ændring af den globale møde politik for din organisation.</span><span class="sxs-lookup"><span data-stu-id="0d04a-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="0d04a-105">Denne cmdlet kræver i øjeblikket brugen af Skype for Business PowerShell-modulet.</span><span class="sxs-lookup"><span data-stu-id="0d04a-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="0d04a-106">For at få konfigureret til at bruge denne cmdlet skal du se [administration af politikker via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="0d04a-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="0d04a-107">Når du har konfigureret en politik, skal du anvende den på brugerne. eller hvis du har ændret den globale politik, gælder den automatisk for brugere.</span><span class="sxs-lookup"><span data-stu-id="0d04a-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="0d04a-108">Du skal vente mindst **4 timer op til 24 timer** , før politikkerne træder i kraft, for at du kan ændre politikken.</span><span class="sxs-lookup"><span data-stu-id="0d04a-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="0d04a-109">Sørg for at gennemgå dokumentationen nedenfor, før du foretager disse ændringer for at forstå, hvad dette giver mulighed for.</span><span class="sxs-lookup"><span data-stu-id="0d04a-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="0d04a-110">Forstå kontrolelementer til politik for mødets informationspolitik</span><span class="sxs-lookup"><span data-stu-id="0d04a-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="0d04a-111">Disse indstillinger styrer, hvilke mødedeltagere der skal vente i informations samarbejdet, før de deltager i mødet, og det tilsvarende omfang de er tilladt i et møde.</span><span class="sxs-lookup"><span data-stu-id="0d04a-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="0d04a-112">Du kan bruge PowerShell til at opdatere indstillinger for møde politik, der endnu ikke er implementeret (kaldet "kommer snart") i teams administration.</span><span class="sxs-lookup"><span data-stu-id="0d04a-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="0d04a-113">Se nedenfor for at få et eksempel på en PowerShell-cmdlet, der gør det muligt for alle brugere at omgå informations funktionen.</span><span class="sxs-lookup"><span data-stu-id="0d04a-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="0d04a-114">Giv [automatisk personer](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) en per-Organizer-politik, der styrer, om personer deltager i et møde direkte eller venter i informations funktionen, indtil de er optaget af en godkendt bruger.</span><span class="sxs-lookup"><span data-stu-id="0d04a-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="0d04a-115">[Tillad, at anonyme personer starter et møde](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) , er en politik om arrangøren, der styrer, om anonyme personer, herunder B2B-og organisations brugere, kan deltage i brugerens møde uden en godkendt bruger fra organisationen i fremmøde.</span><span class="sxs-lookup"><span data-stu-id="0d04a-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="0d04a-116">[Giv opkalds brugere mulighed for at omgå informations](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) udbyderen (**kommer snart**) er en politik om arrangøren, der styrer, om personer, der ringer ind via telefon, kan deltage i mødet direkte eller vente i informations funktionen, uanset om indstillingen Giv **personer automatisk** er blevet givet.</span><span class="sxs-lookup"><span data-stu-id="0d04a-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="0d04a-117">[Tillad, at arrangører kan tilsidesætte informations indstillinger](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**kommer snart**) er en politik om arrangøren, der styrer, om mødearrangøren kan tilsidesætte de informations indstillinger, som en administrator har angivet i **automatisk give personer** **tilladelse til at undgå, at opkalds brugere** går i gang med at planlægge et nyt møde.</span><span class="sxs-lookup"><span data-stu-id="0d04a-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="0d04a-118">**Bemærk:** Læs [Administrer møde politikker i teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for at få en komplet oversigt over møde politikker i Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="0d04a-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
