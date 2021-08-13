---
title: Skift mailadressen for en Microsoft 365-gruppe eller Microsoft Teams
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
ms.openlocfilehash: acb343553bfb7e100c03d0e7046ed5cbdd6b739b9a61e3faf17768bd8aadff34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995616"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Skift mailadressen for en Microsoft 365-gruppe eller Microsoft Teams

Du kan ændre mailadressen for en Microsoft 365-gruppe eller Microsoft Teams ved at bruge [Microsoft 365 Administration](https://admin.microsoft.com/). Markér blot gruppen, og vælg @rediger mailadresse.

Du kan også bruge følgende EXO PowerShell-kommando til at ændre den primære SMTP-adresse for en Microsoft 365-gruppe/Teams:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Eksempel:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
