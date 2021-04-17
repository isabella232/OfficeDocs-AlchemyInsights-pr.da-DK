---
title: Skift mailadresse for en Microsoft 365-gruppe
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
ms.openlocfilehash: 8eaafae8650a8072cdfbec281afe6d5e93fea655
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819038"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Skift mailadresse for en Microsoft 365-gruppe

Du kan ændre mailadressen på en Microsoft 365-gruppe ved hjælp af Administration. Markér blot gruppen, og vælg @rediger mailadresse.

Du kan også bruge følgende EXO PowerShell-kommando til at ændre den primære SMTP-adresse for en Microsoft 365-gruppe:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Eksempel:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
