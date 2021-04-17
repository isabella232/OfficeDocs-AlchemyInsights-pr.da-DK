---
title: Gendan slettede elementer med cmdlet
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
- "1800008"
- "5718"
ms.openlocfilehash: d8f2a50f39d7bcd321692ab093e2efa6613e9814
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835805"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="d2495-102">Gendan slettede elementer med cmdlet</span><span class="sxs-lookup"><span data-stu-id="d2495-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="d2495-103">Brug [cmdlet'en Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) til at få vist slettede elementer i postkasser.</span><span class="sxs-lookup"><span data-stu-id="d2495-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="d2495-104">Når du har fundet de slettede elementer, kan du bruge cmdlet'en [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) til at gendanne dem.</span><span class="sxs-lookup"><span data-stu-id="d2495-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="d2495-105">Se alle oplysninger i [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="d2495-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="d2495-106">Du skal have tildelt rollen Postkasse Import Eksport, før du kan køre denne cmdlet.</span><span class="sxs-lookup"><span data-stu-id="d2495-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="d2495-107">Se [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="d2495-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
