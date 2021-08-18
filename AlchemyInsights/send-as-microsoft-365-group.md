---
title: Send som Microsoft 365 gruppe
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: 204b2c1777f76f11663b2735b784cbb56f1f1aba891628fb46ef37b501c9ff85
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54086122"
---
# <a name="send-as-microsoft-365-group"></a>Send som Microsoft 365 gruppe

Du kan tildele Send som-tilladelser for at tillade bestemte brugere at sende meddelelser som en Microsoft 365 gruppe:  

1. Forbind til Exchange Online PowerShell.  

2. Kør følgende kommando:  

    Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs

Du kan få mere at vide [under Tillad, at medlemmer kan sende som eller sende på vegne af en gruppe.](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide)