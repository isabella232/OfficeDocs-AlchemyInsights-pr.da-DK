---
title: Afsenderen modtager ikke mails, der sendes til Microsoft 365 gruppe
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: 893b80567567590357a638370b8c8d58b87a98a51c68cfcc84629eda5ac71b44
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53958291"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>Afsenderen modtager ikke mails, der sendes til Microsoft 365 gruppe

Som standard modtager afsenderen af en mail til en Microsoft 365-gruppe ikke en kopi af meddelelsen i sin indbakke, selvom afsenderen er medlem af gruppen.

Brug denne EXO PowerShell-kommando til at give afsenderen mulighed for at modtage en kopi af hver mail, vedkommende sender til Microsoft 365 gruppe:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

Sådan aktiveres indstillingen for alle postkasser på én gang:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**Bemærk!** Det kan tage op til en time, før ændringerne i denne indstilling træder i kraft.