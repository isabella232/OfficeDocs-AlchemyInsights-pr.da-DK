---
title: Micro-forsinkelser eller -begrænsning i Exchange Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 55844747be27ea4ff8f538492e576195b3a5f0bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47743908"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="5f021-102">Micro-forsinkelser eller -begrænsning i Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="5f021-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="5f021-103">Du vil muligvis se "Micro-forsinkelse anvendt"-advarsler eller -forsinkelser, når du kører scripts og cmdlets i Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="5f021-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="5f021-104">Her er to forslag til dette:</span><span class="sxs-lookup"><span data-stu-id="5f021-104">Here are two suggestions related to this:</span></span>

- <span data-ttu-id="5f021-105">Det kan være en god ide at prøve at bruge [Exchange Online v2 PowerShell-modul](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), som indeholder CMDlets, der er baseret på REST API, og er betydeligt mere produktiv.</span><span class="sxs-lookup"><span data-stu-id="5f021-105">You might want to try using the [Exchange Online v2 PowerShell module](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="5f021-106">Dette kan være en god løsning til en masse af Get- CMDlets, der ofte anvendes.</span><span class="sxs-lookup"><span data-stu-id="5f021-106">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="5f021-107">Hvis du skal bruge CMDlets, der endnu ikke er omfattet af v2-modulet, skal du se [Køre PowerShell-cmdlets til et stort antal brugere i Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), som taler om, hvordan du løser forventede PowerShell-begrænsninger i Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="5f021-107">If you need to use CMDlets that are not covered in the v2 module yet, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around expected PowerShell throttling limits in Exchange Online.</span></span>
