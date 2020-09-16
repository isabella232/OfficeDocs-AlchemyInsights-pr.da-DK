---
title: Afsenderen modtager ikke mails, der sendes til Microsoft 365-gruppe
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
ms.openlocfilehash: b8091305d55408f51cf369506acc7bfac59defb5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751309"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a><span data-ttu-id="b7c6a-102">Afsenderen modtager ikke mails, der sendes til Microsoft 365-gruppe</span><span class="sxs-lookup"><span data-stu-id="b7c6a-102">Sender does not receive email sent to Microsoft 365 group</span></span>

<span data-ttu-id="b7c6a-103">Som standard modtager afsenderen af en mail til en Microsoft 365-gruppe en kopi af meddelelsen i deres indbakke, selvom afsenderen er medlem af gruppen.</span><span class="sxs-lookup"><span data-stu-id="b7c6a-103">By default, the sender of an email message to a Microsoft 365 group doesn't receive a copy of the message in their Inbox, even if the sender is a member of the group.</span></span>

<span data-ttu-id="b7c6a-104">Brug denne EXO PowerShell-kommando til at give afsenderen tilladelse til at modtage en kopi af hver mail, de sender til Microsoft 365-gruppen:</span><span class="sxs-lookup"><span data-stu-id="b7c6a-104">Use this EXO PowerShell command to allow the sender to receive a copy of each email they send to the Microsoft 365 group:</span></span>  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

<span data-ttu-id="b7c6a-105">Sådan aktiveres indstillingen for alle postkasser på én gang:</span><span class="sxs-lookup"><span data-stu-id="b7c6a-105">To enable the setting for all mailboxes at once:</span></span>

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

<span data-ttu-id="b7c6a-106">**Bemærk!** Ændringer af denne indstilling tager op til en time op til at træde i kraft.</span><span class="sxs-lookup"><span data-stu-id="b7c6a-106">**Note** Changes to this setting take up to an hour to take effect.</span></span>