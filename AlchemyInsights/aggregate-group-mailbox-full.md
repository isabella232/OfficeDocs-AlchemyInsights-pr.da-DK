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
ms.openlocfilehash: 6655bbe9482400eeb3cfdf0b91bdc595e3d98fbff0f6d9244db8bb4dd958305e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951847"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AggregateGroupMailbox fuld NDR modtaget for mails, der sendes Microsoft 365 gruppe

Brug følgende EXO Shell-kommando til at oprette en Exchange-transportregel for automatisk at slippe mails, der sendes til samlet gruppepostkasse:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> Erstat SMTP-adressen i **-SentTo** med SMTP-adressen på den samlede gruppepostkasse i din lejer. Du kan få SMTP-adressen på den samlede gruppepostkasse fra NDR modtaget.



