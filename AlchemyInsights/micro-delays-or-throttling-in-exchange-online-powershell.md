---
title: Micro-forsinkelser eller -begrænsning i Exchange Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 7ab4e7f18b7b8edf08098af8fe9674f66b1b81f4
ms.sourcegitcommit: fbaa2ce2cfb4d56d8c4cf2fa2d95489bdfcb7ff0
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 04/30/2020
ms.locfileid: "43947835"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="b39bd-102">Micro-forsinkelser eller -begrænsning i Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="b39bd-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="b39bd-103">Du vil muligvis se "Micro-forsinkelse anvendt"-advarsler eller -forsinkelser, når du kører scripts og cmdlets i Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="b39bd-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="b39bd-104">Her er to forslag til dette:</span><span class="sxs-lookup"><span data-stu-id="b39bd-104">Here are two suggestions related to this:</span></span>

- <span data-ttu-id="b39bd-105">Det kan være en god ide at prøve at bruge [Exchange Online v2 PowerShell-modul](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), som indeholder CMDlets, der er baseret på REST API, og er betydeligt mere produktiv.</span><span class="sxs-lookup"><span data-stu-id="b39bd-105">You might want to try using the [Exchange Online v2 PowerShell module](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="b39bd-106">Dette kan være en god løsning til en masse af Get- CMDlets, der ofte anvendes.</span><span class="sxs-lookup"><span data-stu-id="b39bd-106">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="b39bd-107">Hvis du skal bruge CMDlets, der endnu ikke er omfattet af v2-modulet, skal du se [Køre PowerShell-cmdlets til et stort antal brugere i Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), som taler om, hvordan du løser forventede PowerShell-begrænsninger i Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="b39bd-107">If you need to use CMDlets that are not covered in the v2 module yet, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around expected PowerShell throttling limits in Exchange Online.</span></span>
