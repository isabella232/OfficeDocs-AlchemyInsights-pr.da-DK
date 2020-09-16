---
title: Gendan slettede elementer med cmdlet'en
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
- "1800008"
- "5718"
ms.openlocfilehash: 91a9bcf75b13881b903a1d3b6f2da53f65811c9c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741297"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="a9d65-102">Gendan slettede elementer med cmdlet'en</span><span class="sxs-lookup"><span data-stu-id="a9d65-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="a9d65-103">Brug cmdlet'en [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) til at få vist slettede elementer i postkasser.</span><span class="sxs-lookup"><span data-stu-id="a9d65-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="a9d65-104">Når du har fundet de slettede elementer, skal du bruge [gendannelses-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) -cmdlet til at gendanne dem.</span><span class="sxs-lookup"><span data-stu-id="a9d65-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="a9d65-105">Se alle detaljer i [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="a9d65-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="a9d65-106">Du skal have tildelt eksport rollen postkasse import, før du kan køre denne cmdlet.</span><span class="sxs-lookup"><span data-stu-id="a9d65-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="a9d65-107">Læs mere [-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="a9d65-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
