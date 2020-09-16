---
title: Skift mailadresse for en Microsoft 365-gruppe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: a2605bcd66f61de811ebb6e273e4ef1cff2b0119
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47733681"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Skift mailadresse for en Microsoft 365-gruppe

Du kan ændre mailadressen til en Microsoft 365-gruppe ved hjælp af administrations centeret. Du skal bare markere gruppen og vælge @edit mailadresse.

Du kan også bruge følgende EXO PowerShell-kommando til at ændre den primære SMTP-adresse for en Microsoft 365-gruppe:

Set-Unifiedgrouphttps <Group Name> -PrimarySmtpAddress <new SMTP Address>

:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
