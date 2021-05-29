---
title: Micro-forsinkelser eller -begrænsning i Exchange Online PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702120"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="e1a47-102">Micro-forsinkelser eller -begrænsning i Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="e1a47-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="e1a47-103">Du vil muligvis se "Micro-forsinkelse anvendt"-advarsler eller -forsinkelser, når du kører scripts og cmdlets i Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="e1a47-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="e1a47-104">Her er nogle forslag til, hvordan du kan løse dette:</span><span class="sxs-lookup"><span data-stu-id="e1a47-104">Here are a few suggestions how to solve this:</span></span>

- <span data-ttu-id="e1a47-105">Kør vores diagnosticeringsværktøj for at slappe af din lejers PowerShell-begrænsningspolitikker.</span><span class="sxs-lookup"><span data-stu-id="e1a47-105">Please run our diagnostics to relax your tenant's PowerShell throttling policies.</span></span> <span data-ttu-id="e1a47-106">Denne løsning løser problemet for de fleste.</span><span class="sxs-lookup"><span data-stu-id="e1a47-106">This solution will solve the problem for most.</span></span>
- <span data-ttu-id="e1a47-107">Hvis problemet stadig ikke løses, kan du bruge [Exchange Online v2 PowerShell-modulet,](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)som indeholder CMDlet'er, der er baseret på REST-API, og som er væsentligt mere performant.</span><span class="sxs-lookup"><span data-stu-id="e1a47-107">If issue still not solved, use the [Exchange Online v2 PowerShell module](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="e1a47-108">Dette kan være en god løsning til en masse af Get- CMDlets, der ofte anvendes.</span><span class="sxs-lookup"><span data-stu-id="e1a47-108">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="e1a47-109">Hvis du skal bruge CMDlet'er, der ikke er dækket af v2-modulet, skal du se Køre [PowerShell-cmdlet'er for](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)et stort antal brugere i Office 365 , som handler om, hvordan du kommer uden om PowerShell-begrænsningsgrænser i Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="e1a47-109">If you need to use CMDlets that are not covered in the v2 module, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around PowerShell throttling limits in Exchange Online.</span></span>
