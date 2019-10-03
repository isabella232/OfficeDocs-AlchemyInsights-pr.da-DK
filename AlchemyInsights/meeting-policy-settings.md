---
title: Indstillinger for møde politik
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: dac06690b51459ca166c15a5ef0f4c7e7a6d36f0
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376580"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="d342d-102">Administrer møde politikker i Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="d342d-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="d342d-103">Møde politikker bruges til at styre de funktioner, der er tilgængelige for mødedeltagere til møder, der er planlagt af brugere i organisationen.</span><span class="sxs-lookup"><span data-stu-id="d342d-103">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="d342d-104">Nogle funktioner i møde politikker er muligvis ikke implementeret i teams administration endnu (disse er mærket "kommer snart" i dokumentationen).</span><span class="sxs-lookup"><span data-stu-id="d342d-104">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="d342d-105">I dette tilfælde, eller hvis du får en fejl som "vi kan ikke opdatere politikken lige nu, men prøv igen senere" i Microsoft teams administration, anbefaler vi, at du bruger PowerShell til at oprette eller redigere teams-møde politikker.</span><span class="sxs-lookup"><span data-stu-id="d342d-105">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="d342d-106">Du finder flere oplysninger om møde politikker i følgende ressourcer:</span><span class="sxs-lookup"><span data-stu-id="d342d-106">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="d342d-107">Du kan få mere at vide om at oprette politikker, foretage ændringer og tildele brugere til politikken under [administrere møde politikker i teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="d342d-107">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="d342d-108">Hvis du vil foretage politikændringer ved hjælp af PowerShell-cmdlets, skal du se [Oversigt i teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)</span><span class="sxs-lookup"><span data-stu-id="d342d-108">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="d342d-109">Du skal bruge [Skype for Business PowerShell-modulet](https://www.microsoft.com/download/details.aspx?id=39366) til teams-møde politikker.</span><span class="sxs-lookup"><span data-stu-id="d342d-109">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="d342d-110">Se [dokumentationen til cmdlet'er \*-csteamsmeetingpolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for at fÃ ¥ flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="d342d-110">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

<span data-ttu-id="d342d-111">**Bemærk:** Det kan tage op til 24 timer, at politikændringer træder i kraft for brugerne.</span><span class="sxs-lookup"><span data-stu-id="d342d-111">**Note:** It can take up to 24 hours for policy changes to take effect for users.</span></span> <span data-ttu-id="d342d-112">Du vil muligvis ikke kunne foretage ændringer af nyoprettede politikker med det samme. Vent 4 timer, og forsøg at ændre en nyoprettet politik igen.</span><span class="sxs-lookup"><span data-stu-id="d342d-112">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span> <span data-ttu-id="d342d-113">Hvis du stadig har problemer, kan du prøve PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d342d-113">If you're still having problems, try PowerShell.</span></span>  