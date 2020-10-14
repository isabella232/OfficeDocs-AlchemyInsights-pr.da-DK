---
title: Send som mail med aktiveret offentlig mappe i EXO
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: ed62c6d7db0ae532f806ce4fdc48f42623bcd545
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/13/2020
ms.locfileid: "48461840"
---
# <a name="sendas-mail-enabled-public-folder"></a>SendAs mail-aktiveret offentlig mappe

I følgende eksempel tildeles tilladelserne "Send som" til den offentlige mappe, der er aktiveret for mail NewPF1, til bruger Jason.

Add-RecipientPermission-Identity ' NewPF1 '-trustee "Jason"-AccessRights ' SendAs '

Du kan finde detaljerede oplysninger om syntaks og parameter under [Tildel tilladelserne "Send som" eller "Send på vegne af" til mailaktiverede offentlige mapper](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).

