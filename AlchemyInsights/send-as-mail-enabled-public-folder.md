---
title: Offentlig mappe med aktiveret send som mail i EXO
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
ms.openlocfilehash: 22aa3e8f46c2ff4f62cb520b9498041dffb9d3a3eb607d788cc97b10bf32dbb5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052560"
---
# <a name="sendas-mail-enabled-public-folder"></a>Public Folder aktiveret i SendAs Mail

I følgende eksempel tildeles "Send som"-tilladelser for den mailaktiverede offentlige mappe NewPF1 til brugeren Jason.

Add-RecipientPermission -Identity 'NewPF1' -Trustee "Jason" -AccessRights 'SendAs'

Du kan finde detaljerede oplysninger om syntaks og parameter i Tildele tilladelserne "Send som" eller "Send på vegne [af" til mailaktiverede offentlige mapper.](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs)

