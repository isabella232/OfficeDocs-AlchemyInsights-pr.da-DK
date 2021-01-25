---
title: Din Arkiv postkasse er næsten fuld
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974275"
---
# <a name="your-archive-mailbox-is-almost-full"></a><span data-ttu-id="502bb-102">Din Arkiv postkasse er næsten fuld</span><span class="sxs-lookup"><span data-stu-id="502bb-102">Your archive mailbox is almost full</span></span>

<span data-ttu-id="502bb-103">Hvis brugeren modtager advarslen. **Din postkasse er næsten fuld**, eller du har brug for at øge størrelsen på postkassen i deres arkiv, da her er nogle tip:</span><span class="sxs-lookup"><span data-stu-id="502bb-103">If the user receives the warning; **Your archive mailbox is almost full**, or you need to increase the size of their archive mailbox, here are some tips:</span></span>

1. <span data-ttu-id="502bb-104">Hvis brugeren er tildelt en Exchange Online-plan 1, skal du opgradere til **Exchange Online plan 2** -licens for at øge størrelsen fra 50 GB til 100 GB.</span><span class="sxs-lookup"><span data-stu-id="502bb-104">If the user is assigned an Exchange Online Plan 1, upgrade to **Exchange Online Plan 2** license to increase the size from 50 GB to 100GB.</span></span>
1. <span data-ttu-id="502bb-105">Hvis brugeren allerede er tildelt en af følgende: **Exchange Online plan 2** eller en Exchange Online-plan 1 med et tilføjelsesprogram til Exchange Online-arkivering, skal du følge nedenstående trin for at aktivere automatisk udvidelse af arkivering:.</span><span class="sxs-lookup"><span data-stu-id="502bb-105">If the user is already assigned either of the following: **Exchange Online Plan 2** or an Exchange Online Plan 1 with an Exchange Online Archiving add-on, use the steps below to enable Auto-Expanding archiving:.</span></span>
 
    1. <span data-ttu-id="502bb-106">[Opret forbindelse til Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="502bb-106">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span></span>
    2. <span data-ttu-id="502bb-107">Kør følgende Group for brugeren:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span><span class="sxs-lookup"><span data-stu-id="502bb-107">Run the following commandlet for the user:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span></span>
    1. <span data-ttu-id="502bb-108">Kør følgende Group for at bekræfte, at den er aktiveret for brugeren:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span><span class="sxs-lookup"><span data-stu-id="502bb-108">Run the following commandlet to confirm it is enabled for the user:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span></span>

<span data-ttu-id="502bb-109">Du kan finde flere oplysninger under:</span><span class="sxs-lookup"><span data-stu-id="502bb-109">For more information see:</span></span>

- [<span data-ttu-id="502bb-110"> Aktivér ubegrænset arkivering – hjælp til administratorer-Microsoft 365-kompatibilitet | Microsoft-dokumenter</span><span class="sxs-lookup"><span data-stu-id="502bb-110"> Enable unlimited archiving - Admin Help - Microsoft 365 Compliance | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [<span data-ttu-id="502bb-111">Exchange Online-begrænsninger – service beskrivelser | Microsoft-dokumenter</span><span class="sxs-lookup"><span data-stu-id="502bb-111">Exchange Online limits - Service Descriptions | Microsoft Docs</span></span>](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [<span data-ttu-id="502bb-112">Opgrader til en anden virksomhedsplan | Microsoft-dokumenter</span><span class="sxs-lookup"><span data-stu-id="502bb-112">Upgrade to a different business plan | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

