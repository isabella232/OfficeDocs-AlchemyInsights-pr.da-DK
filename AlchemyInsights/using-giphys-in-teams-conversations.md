---
title: Brug af Giphys i team samtaler
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982461"
---
# <a name="using-giphys-in-teams-conversations"></a><span data-ttu-id="2edff-102">Brug af Giphys i team samtaler</span><span class="sxs-lookup"><span data-stu-id="2edff-102">Using Giphys in Teams Conversations</span></span>

<span data-ttu-id="2edff-103">Giphys adgang i team chat er aktiveret som standard.</span><span class="sxs-lookup"><span data-stu-id="2edff-103">Giphys access in Teams chat is enabled by default.</span></span> <span data-ttu-id="2edff-104">Som administrator kan du kontrollere, om Giphys er tilgængelige for brugerne, ved at [angive en meddelelses politik](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) og sikre, at **brugen af Giphys i samtaler** er **slået til**.</span><span class="sxs-lookup"><span data-stu-id="2edff-104">As an administrator, you can control if Giphys are available to users by [setting a messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) and ensuring that **Use Giphys in conversations** is **On**.</span></span>

<span data-ttu-id="2edff-105">Hvis GIF-filer ikke fungerer som forventet i team samtaler, skal du kontrollere:</span><span class="sxs-lookup"><span data-stu-id="2edff-105">If GIFs are not working as expected in Teams conversations, verify:</span></span>

<span data-ttu-id="2edff-106">[Meddelelses politikken](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) skal tillade Giphys.</span><span class="sxs-lookup"><span data-stu-id="2edff-106">The [messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) needs to allow Giphys.</span></span> <span data-ttu-id="2edff-107">Sådan bekræfter du ved hjælp af PowerShell-cmdletter:</span><span class="sxs-lookup"><span data-stu-id="2edff-107">To verify by using PowerShell cmdlets:</span></span>

- <span data-ttu-id="2edff-108">Kontrollér, at du kan [administrere teams med PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="2edff-108">Verify that you can [Manage Teams with PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span></span>
- <span data-ttu-id="2edff-109">Kør PowerShell-kommandoen [Get-CsTeamsMessagingPolicy-Identity global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) , og kontrollér, at **AllowGiphy** er angivet til **sand**.</span><span class="sxs-lookup"><span data-stu-id="2edff-109">Run the PowerShell command [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) and verify that **AllowGiphy** is set to **TRUE**.</span></span>
- <span data-ttu-id="2edff-110">Hvis **AllowGiphy** er indstillet til **falsk** , skal du køre følgende PowerShell [-kommando set-CsTeamsMessagingPolicy-Identity global-AllowGiphy $true](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="2edff-110">If **AllowGiphy** is set to **FALSE** , run the following PowerShell command [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span></span>

<span data-ttu-id="2edff-111">[Valgfrie forbundne oplevelser](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) skal være aktiveret, for at du kan få adgang til Giphy-URL-adressen.</span><span class="sxs-lookup"><span data-stu-id="2edff-111">[Optional Connected Experiences](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) need to be enabled to allow access to the Giphy URL.</span></span>

> [!NOTE]
> <span data-ttu-id="2edff-112">Hvis du har flere teams-meddelelses politikker konfigureret for din lejer, kan du bestemme identiteten af den politik, der er tildelt den påvirkede bruger, med PowerShell [-kommandoen Get-CsOnlineUser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Vælg TeamsMessagingPolicy.</span><span class="sxs-lookup"><span data-stu-id="2edff-112">If you have multiple Teams Messaging policies configured for your tenant, you can determine the identity of the policy assigned to the impacted user with the PowerShell command [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Select TeamsMessagingPolicy.</span></span>
