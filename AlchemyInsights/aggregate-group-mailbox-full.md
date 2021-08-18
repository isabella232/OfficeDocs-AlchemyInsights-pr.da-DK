---
title: AggregateGroupMailbox fuld NDR modtaget for mails, der sendes Microsoft 365 gruppe
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004286"
- "7656"
ms.openlocfilehash: ace8e256e3771f82512abcb9e20b832381eedf80
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315904"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AggregateGroupMailbox fuld NDR modtaget for mails, der sendes Microsoft 365 gruppe

Brug følgende EXO Shell-kommando til at oprette en Exchange-transportregel for automatisk at slippe mails, der sendes til samlet gruppepostkasse:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

**Bemærk!** Erstat SMTP-adressen i **-SentTo med** SMTP-adressen på den samlede gruppepostkasse i din lejer. Du kan få SMTP-adressen på den samlede gruppepostkasse fra NDR modtaget.



