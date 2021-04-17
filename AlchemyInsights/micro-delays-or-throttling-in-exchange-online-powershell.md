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
ms.openlocfilehash: 680df9e6e2404ff6b60b17d6ac88e202e9a7bb25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830027"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="79cfb-102">Micro-forsinkelser eller -begrænsning i Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="79cfb-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="79cfb-103">Du vil muligvis se "Micro-forsinkelse anvendt"-advarsler eller -forsinkelser, når du kører scripts og cmdlets i Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="79cfb-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="79cfb-104">Her er to forslag til dette:</span><span class="sxs-lookup"><span data-stu-id="79cfb-104">Here are two suggestions related to this:</span></span>

- <span data-ttu-id="79cfb-105">Det kan være en god ide at prøve at bruge [Exchange Online v2 PowerShell-modul](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), som indeholder CMDlets, der er baseret på REST API, og er betydeligt mere produktiv.</span><span class="sxs-lookup"><span data-stu-id="79cfb-105">You might want to try using the [Exchange Online v2 PowerShell module](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="79cfb-106">Dette kan være en god løsning til en masse af Get- CMDlets, der ofte anvendes.</span><span class="sxs-lookup"><span data-stu-id="79cfb-106">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="79cfb-107">Hvis du skal bruge CMDlets, der endnu ikke er omfattet af v2-modulet, skal du se [Køre PowerShell-cmdlets til et stort antal brugere i Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), som taler om, hvordan du løser forventede PowerShell-begrænsninger i Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="79cfb-107">If you need to use CMDlets that are not covered in the v2 module yet, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around expected PowerShell throttling limits in Exchange Online.</span></span>
