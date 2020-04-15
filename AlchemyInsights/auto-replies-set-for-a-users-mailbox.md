---
title: Indstil autosvar for en postkasse
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: aeeb2e1e76fe602d2767b422797452fd1155fdd5
ms.sourcegitcommit: fdfd41c2bfb2d45003b3906e6469377384a91cb5
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2020
ms.locfileid: "43509488"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Indstil autosvar for en brugers postkasse

**Metode 1**

1. Log på Office 365-portalen.

2. Gå til **Brugere > Aktive brugere** (eller **Grupper > Delte postkasser**, hvis du indstiller dette for en delt postkasse).

3. Vælg en bruger, der har en Microsoft Exchange-postkasse.

4. I menuen, der kommer frem i højre side, skal du gå til **Mailindstillinger > Autosvar** (hvis det er en delt postkasse, skal du blot klikke på **Autosvar** i menuen).

**Metode 2**

1. Log på Office 365-administratorportalen ved hjælp af legitimationsoplysninger for administrator.

2. Udvid **Administration**, og klik derefter på **Exchange**.

3. Klik på billedet i øverste højre hjørne, klik på **En anden bruger**, og vælg derefter den brugerpostkasse, du vil ændre.

4. I venstre side skal du vælge **Indstillinger**, klikke på **Organiser mails** og derefter klikke på **Autosvar.**

**Metode 3**

Kør følgende cmdlet i Exchange Online PowerShell:

PowerShellCopy

```
    Set-MailboxAutoReplyConfiguration
```

Se [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration) for at få mere at vide om denne cmdlet.
