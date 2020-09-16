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
# <a name="recover-deleted-items-with-cmdlet"></a>Gendan slettede elementer med cmdlet'en

- Brug cmdlet'en [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) til at få vist slettede elementer i postkasser. Når du har fundet de slettede elementer, skal du bruge [gendannelses-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) -cmdlet til at gendanne dem.

- Se alle detaljer i [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).

- Du skal have tildelt eksport rollen postkasse import, før du kan køre denne cmdlet. Læs mere [-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for at få flere oplysninger.
