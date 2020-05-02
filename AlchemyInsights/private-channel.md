---
title: Privat kanal
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005432"
---
# <a name="private-channels-in-microsoft-teams"></a><span data-ttu-id="5bafd-102">Private kanaler i Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="5bafd-102">Private channels in Microsoft Teams</span></span>

<span data-ttu-id="5bafd-103">Private kanaler er en ny funktion i Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="5bafd-103">Private channels is a new feature in Microsoft Teams.</span></span> <span data-ttu-id="5bafd-104">Bemærk, at private kanaler ikke kan konverteres fra standardkanaler eller omvendt.</span><span class="sxs-lookup"><span data-stu-id="5bafd-104">Note that private channels cannot be converted from standard channels or vice versa.</span></span>

<span data-ttu-id="5bafd-105">Du kan finde flere oplysninger [private channel creation and membership](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) om private kanaler, [private channel SharePoint sites](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites) [f.eks.](https://docs.microsoft.com/MicrosoftTeams/private-channels)</span><span class="sxs-lookup"><span data-stu-id="5bafd-105">For details about private channels, such as information on [private channel creation and membership](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) and [private channel SharePoint sites](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), see [Private channels in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span></span> 

<span data-ttu-id="5bafd-106">**Bemærk:** Da konfiguration til opbevaring af private kanalmeddelelser endnu ikke understøttes, vil lejere med opbevaringspolitikker aktiveret ikke have private kanaler aktiveret som standard.</span><span class="sxs-lookup"><span data-stu-id="5bafd-106">**Note:** Because configuration for retention of private channel messages is not yet supported, tenants with retention policies enabled will not have private channels enabled by default.</span></span> <span data-ttu-id="5bafd-107">Private kanaler kan aktiveres i Teams Administration.</span><span class="sxs-lookup"><span data-stu-id="5bafd-107">Private channels can be enabled in the Teams admin center.</span></span> <span data-ttu-id="5bafd-108">Bemærk også, at selvom opbevaring af private kanalbeskeder ikke understøttes, understøttes opbevaring af filer, der deles i private kanaler.</span><span class="sxs-lookup"><span data-stu-id="5bafd-108">Also, note that while retention of private channel messages is not supported, retention of files shared in private channels is supported.</span></span>

<span data-ttu-id="5bafd-109">**Har du brug for en ny teamejer?**</span><span class="sxs-lookup"><span data-stu-id="5bafd-109">**Need a new team owner?**</span></span>

<span data-ttu-id="5bafd-110">Hvis din private kanalejer forlader den, kan du tilføje en ny teamejer via Teams Powershell.</span><span class="sxs-lookup"><span data-stu-id="5bafd-110">If your private channel owner leaves, you can add a new team owner via Teams Powershell.</span></span>


- <span data-ttu-id="5bafd-111">Gå [her](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) for at installere Teams Powershell.</span><span class="sxs-lookup"><span data-stu-id="5bafd-111">Go [here](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) to install Teams Powershell.</span></span>

<span data-ttu-id="5bafd-112">Her er den cmdlet, du skal bruge:</span><span class="sxs-lookup"><span data-stu-id="5bafd-112">Here is the cmdlet you will need:</span></span>

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

<span data-ttu-id="5bafd-113">Yderligere oplysninger om Teams Powershell finder du i [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="5bafd-113">For more information on Teams Powershell, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span>
