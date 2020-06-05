---
title: Ændre mailadressen på en Microsoft 365-gruppe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580651"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Ændre mailadressen på en Microsoft 365-gruppe

Du kan ændre mailadressen på en Microsoft 365-gruppe ved hjælp af Administration. Du skal blot vælge gruppen og vælge @edit e-mail-adresse.

Du kan også bruge følgende EXO PowerShell-kommando til at ændre den primære SMTP-adresse for en Microsoft 365-gruppe:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address>

Eksempel:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
