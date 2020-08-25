---
title: Afsenderen modtager ikke mails, der sendes til Microsoft 365-gruppe
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b3b438e17c35f18289d3e9c3ca89d16a6f2a065f
ms.sourcegitcommit: dcca0df53f9194f406cf3a5f6b046cb33a0a5b03
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/21/2020
ms.locfileid: "46871698"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>Afsenderen modtager ikke mails, der sendes til Microsoft 365-gruppe

Som standard modtager afsenderen af en mail til en Microsoft 365-gruppe en kopi af meddelelsen i deres indbakke, selvom afsenderen er medlem af gruppen.

Brug denne EXO PowerShell-kommando til at give afsenderen tilladelse til at modtage en kopi af hver mail, de sender til Microsoft 365-gruppen:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

Sådan aktiveres indstillingen for alle postkasser på én gang:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**Bemærk!** Ændringer af denne indstilling tager op til en time op til at træde i kraft.