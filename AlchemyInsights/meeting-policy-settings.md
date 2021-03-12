---
title: Indstillinger for mødepolitik
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
ms.openlocfilehash: 24a55417df0f89063fbdd9ade6d104be4f8ab49c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704600"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="8eb35-102">Administrer mødepolitikker i Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="8eb35-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="8eb35-103">**Bemærk! Det kan tage op til 24 timer, før ændringerne i politikken træder i kraft for brugerne.**</span><span class="sxs-lookup"><span data-stu-id="8eb35-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="8eb35-104">Du kan muligvis ikke foretage ændringer i nyligt oprettede politikker med det samme. vent 4 timer, og forsøg at ændre en nyoprettet politik igen.</span><span class="sxs-lookup"><span data-stu-id="8eb35-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="8eb35-105">Mødepolitikker bruges til at styre de funktioner, der er tilgængelige for mødedeltagere til møder, der planlægges af brugerne i organisationen.</span><span class="sxs-lookup"><span data-stu-id="8eb35-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="8eb35-106">Nogle funktioner i mødepolitikker er muligvis ikke blevet implementeret i Teams Administration endnu (disse er mærket "Kommer snart" i dokumentationen).</span><span class="sxs-lookup"><span data-stu-id="8eb35-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="8eb35-107">I dette tilfælde, eller hvis du får en fejl som "Vi kan ikke opdatere politikken lige nu, men prøv det igen senere" i Microsoft Teams Administration, anbefaler vi, at du bruger PowerShell til at oprette eller redigere teams-mødepolitikker.</span><span class="sxs-lookup"><span data-stu-id="8eb35-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="8eb35-108">Du kan finde flere oplysninger om mødepolitikker i følgende ressourcer:</span><span class="sxs-lookup"><span data-stu-id="8eb35-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="8eb35-109">Hvis du vil have mere at vide om at oprette politikker, foretage ændringer og tildele brugere til politikken, skal du [se Administrer mødepolitikker i Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="8eb35-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="8eb35-110">Hvis du vil foretage politikændringer ved hjælp af PowerShell-cmdlet'er, skal du [se Oversigt over Teams PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)</span><span class="sxs-lookup"><span data-stu-id="8eb35-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="8eb35-111">Du skal bruge [Skype for Business PowerShell-modulet til](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) teams-mødepolitikker.</span><span class="sxs-lookup"><span data-stu-id="8eb35-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="8eb35-112">Gennemgå [dokumentationen til \*-CsTeamsMeetingPolicy cmdlet'er](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="8eb35-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

