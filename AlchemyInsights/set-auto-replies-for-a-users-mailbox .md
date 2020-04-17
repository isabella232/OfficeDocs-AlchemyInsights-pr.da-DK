---
title: Indstil autosvar for en brugers postkasse
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
ms.openlocfilehash: e3cc01298c10fd3ba21327a7fb5cc5396d0ad74d
ms.sourcegitcommit: 23e5b94f1758bfe202008384e300b81816975375
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 04/14/2020
ms.locfileid: "43506454"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Indstil autosvar for en brugers postkasse

**Metode 1**

1. Log på Office 365-portalen.

2. Gå til **Brugere > Aktive brugere** (eller **Grupper > Delte postkasser**, hvis du indstiller dette for en delt postkasse).

3. Vælg en bruger, der har en Microsoft Exchange-postkasse.

4. I menuen, der kommer frem i højre side, skal du gå til **Mailindstillinger > Autosvar** (hvis det er en delt postkasse, skal du blot klikke på **Autosvar** i menuen).

**Metode 2**

1. Log på Office 365-administratorportalen ved hjælp af administratorens legitimationsoplysninger.

2. Udvid **Administration**, og klik derefter på **Exchange**.

3. Klik på billedet i øverste højre hjørne, klik på **En anden bruger**, og vælg derefter den brugerpostkasse, du vil ændre.

4. I venstre side skal du vælge **Indstillinger**, klikke på **Organiser mails** og derefter klikke på **Autosvar.**

**Metode 3**

Kør følgende cmdlet i Exchange Online PowerShell:

PowerShellCopy

    Set-MailboxAutoReplyConfiguration

Du kan finde flere oplysninger om denne cmdlet under [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).
