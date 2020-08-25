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
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a><span data-ttu-id="df6ce-102">Afsenderen modtager ikke mails, der sendes til Microsoft 365-gruppe</span><span class="sxs-lookup"><span data-stu-id="df6ce-102">Sender does not receive email sent to Microsoft 365 group</span></span>

<span data-ttu-id="df6ce-103">Som standard modtager afsenderen af en mail til en Microsoft 365-gruppe en kopi af meddelelsen i deres indbakke, selvom afsenderen er medlem af gruppen.</span><span class="sxs-lookup"><span data-stu-id="df6ce-103">By default, the sender of an email message to a Microsoft 365 group doesn't receive a copy of the message in their Inbox, even if the sender is a member of the group.</span></span>

<span data-ttu-id="df6ce-104">Brug denne EXO PowerShell-kommando til at give afsenderen tilladelse til at modtage en kopi af hver mail, de sender til Microsoft 365-gruppen:</span><span class="sxs-lookup"><span data-stu-id="df6ce-104">Use this EXO PowerShell command to allow the sender to receive a copy of each email they send to the Microsoft 365 group:</span></span>  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

<span data-ttu-id="df6ce-105">Sådan aktiveres indstillingen for alle postkasser på én gang:</span><span class="sxs-lookup"><span data-stu-id="df6ce-105">To enable the setting for all mailboxes at once:</span></span>

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

<span data-ttu-id="df6ce-106">**Bemærk!** Ændringer af denne indstilling tager op til en time op til at træde i kraft.</span><span class="sxs-lookup"><span data-stu-id="df6ce-106">**Note** Changes to this setting take up to an hour to take effect.</span></span>