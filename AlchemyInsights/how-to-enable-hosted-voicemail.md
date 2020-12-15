---
title: Sådan aktiveres hosted voicemail
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/09/2020
ms.locfileid: "49677336"
---
# <a name="how-to-enable-hosted-voicemail"></a><span data-ttu-id="1a885-102">Sådan aktiveres hosted voicemail</span><span class="sxs-lookup"><span data-stu-id="1a885-102">How to enable Hosted Voicemail</span></span>

<span data-ttu-id="1a885-103">Hvis du vil aktivere voicemail, skal du angive **HostedVoicemail** til $true.</span><span class="sxs-lookup"><span data-stu-id="1a885-103">To enable Voicemail, **HostedVoicemail** must be set to $true.</span></span>

<span data-ttu-id="1a885-104">Egenskaben **HostedVoicemail** for brugeren ved hjælp af Remote POWERSHELL (RPS).</span><span class="sxs-lookup"><span data-stu-id="1a885-104">The **HostedVoicemail** property on the user using Remote PowerShell (RPS).</span></span>

<span data-ttu-id="1a885-105">Du kan finde flere oplysninger om at oprette forbindelse til RPS i [Microsoft teams PowerShell-oversigt](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for at få flere oplysninger om at oprette forbindelse til RPS.</span><span class="sxs-lookup"><span data-stu-id="1a885-105">For more information on connecting to RPS, see [Microsoft Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for more information on connecting to RPS.</span></span>

1. <span data-ttu-id="1a885-106">Teams-administratoren skal være logget på Remote PowerShell til teams.</span><span class="sxs-lookup"><span data-stu-id="1a885-106">The Teams Admin should be logged into Remote PowerShell for Teams.</span></span>
1. <span data-ttu-id="1a885-107">Fra PowerShell-Spørg teams-administratoren kan køre **set-csuser User@contoso.com-$true HostedVoiceMail** , hvor SIP-URI'en er for den pågældende bruger.</span><span class="sxs-lookup"><span data-stu-id="1a885-107">From PowerShell prompt the Teams Admin can run **set-csuser user@contoso.com -HostedVoiceMail $true** where the sip uri is of the user in question.</span></span>

> [!NOTE]
> <span data-ttu-id="1a885-108">Ændringer af politikker kan tage op til 24 timer at replikere.</span><span class="sxs-lookup"><span data-stu-id="1a885-108">Changes to policies can take up to 24 hours to replicate.</span></span>