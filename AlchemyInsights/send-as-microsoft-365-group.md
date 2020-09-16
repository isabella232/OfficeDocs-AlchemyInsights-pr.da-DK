---
title: Send som Microsoft 365-gruppe
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
ms.openlocfilehash: 51bd8a10c3da23941cc16d7ba860406f8477044a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740145"
---
# <a name="send-as-microsoft-365-group"></a><span data-ttu-id="12e9a-102">Send som Microsoft 365-gruppe</span><span class="sxs-lookup"><span data-stu-id="12e9a-102">Send As Microsoft 365 group</span></span>

<span data-ttu-id="12e9a-103">Du kan tildele tilladelsen "Send som" for bestemte brugere, så de kan sende meddelelser som en Microsoft 365-gruppe:</span><span class="sxs-lookup"><span data-stu-id="12e9a-103">You can assign Send As permissions to allow specific users to send messages as a Microsoft 365 group:</span></span>  

1. <span data-ttu-id="12e9a-104">Opret forbindelse til Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="12e9a-104">Connect to Exchange Online PowerShell.</span></span>  

2. <span data-ttu-id="12e9a-105">Kør følgende kommando:</span><span class="sxs-lookup"><span data-stu-id="12e9a-105">Run the following command:</span></span>  

    <span data-ttu-id="12e9a-106">Add-RecipientPermission `<GroupName>` -trustee `<MailboxName>` -AccessRights SendAs</span><span class="sxs-lookup"><span data-stu-id="12e9a-106">Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs</span></span>

<span data-ttu-id="12e9a-107">Hvis du vil have mere at vide, skal du se [Giv medlemmer tilladelse til at sende som eller sende på vegne af en gruppe](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="12e9a-107">For more information, see [Allow members to send as or send on behalf of a group](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).</span></span>