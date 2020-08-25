---
title: Send som Microsoft 365-gruppe
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: cfb4bd5ce59eeccdd0812d013b8a444aebeb1d4c
ms.sourcegitcommit: 9818d3c8e6b10f23244e51286e2463caf48fffd5
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/21/2020
ms.locfileid: "46871700"
---
# <a name="send-as-microsoft-365-group"></a>Send som Microsoft 365-gruppe

Du kan tildele tilladelsen "Send som" for bestemte brugere, så de kan sende meddelelser som en Microsoft 365-gruppe:  

1. Opret forbindelse til Exchange Online PowerShell.  

2. Kør følgende kommando:  

    Add-RecipientPermission `<GroupName>` -trustee `<MailboxName>` -AccessRights SendAs

Hvis du vil have mere at vide, skal du se [Giv medlemmer tilladelse til at sende som eller sende på vegne af en gruppe](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).