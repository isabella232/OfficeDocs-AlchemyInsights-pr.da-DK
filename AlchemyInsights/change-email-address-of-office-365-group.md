---
title: Ændre mailadressen på en Microsoft 365 gruppe
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 6bd9301b983d09f6a0058fee17577b9fc695458ed205f96aacf79a87e4a91e34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930723"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Ændre mailadressen på en Microsoft 365 gruppe

Du kan ændre mailadressen på en Microsoft 365 ved hjælp af Administration. Markér blot gruppen, og vælg @rediger mailadresse.

Du kan også bruge følgende EXO PowerShell-kommando til at ændre den primære SMTP-adresse for Microsoft 365 gruppe:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Eksempel:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
