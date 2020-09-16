---
title: Indstillinger for møde politik
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
- "9000734"
- "2657"
ms.openlocfilehash: 683ca12c8f6e2511311c10ab5c4599ee66c08eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794328"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="ef2e7-102">Administrere møde politikker i Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="ef2e7-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="ef2e7-103">**Bemærk: der kan gå op til 24 timer, før politikændringer træder i kraft for brugere.**</span><span class="sxs-lookup"><span data-stu-id="ef2e7-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="ef2e7-104">Du vil muligvis ikke kunne foretage ændringer i nyligt oprettede politikker med det samme. Vent 4 timer, og prøv at ændre en nyoprettet politik igen.</span><span class="sxs-lookup"><span data-stu-id="ef2e7-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="ef2e7-105">Møde politikker bruges til at styre de funktioner, der er tilgængelige for mødedeltagere for møder, der er planlagt af brugere i organisationen.</span><span class="sxs-lookup"><span data-stu-id="ef2e7-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="ef2e7-106">Nogle funktioner i møde politikker er muligvis ikke implementeret i teams administration endnu (de hedder "kommer snart" i dokumentationen).</span><span class="sxs-lookup"><span data-stu-id="ef2e7-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="ef2e7-107">I dette tilfælde eller hvis du får vist en fejlmeddelelse om, at vi ikke kan opdatere politikken lige nu, men prøv igen senere "i Microsoft teams administration, anbefaler vi, at du bruger PowerShell til at oprette eller redigere teams-møde politikker.</span><span class="sxs-lookup"><span data-stu-id="ef2e7-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="ef2e7-108">Du kan finde flere oplysninger om møde politikker i følgende ressourcer:</span><span class="sxs-lookup"><span data-stu-id="ef2e7-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="ef2e7-109">Hvis du vil have mere at vide om at oprette politikker, foretage ændringer og tildele brugere til politikken, skal du se [administrere møde politikker i teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="ef2e7-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="ef2e7-110">Hvis du vil udføre politikændringer ved hjælp af PowerShell-cmdletter, skal du se [Oversigt over teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="ef2e7-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="ef2e7-111">Du skal bruge [Skype for Business PowerShell-modulet](https://www.microsoft.com/download/details.aspx?id=39366) til teams-møde politikker.</span><span class="sxs-lookup"><span data-stu-id="ef2e7-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="ef2e7-112">Gennemse [dokumentationen til \*-CsTeamsMeetingPolicy-cmdletter](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="ef2e7-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

