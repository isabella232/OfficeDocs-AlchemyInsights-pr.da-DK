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
ms.openlocfilehash: 7800a447c5dfcc8397121e1149921916ff7944ac
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819074"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Skift mailadressen for en Microsoft 365-gruppe eller Microsoft Teams

Du kan ændre mailadressen for en Microsoft 365-gruppe eller Microsoft Teams ved at bruge [Microsoft 365 Administration](https://admin.microsoft.com/). Markér blot gruppen, og vælg @rediger mailadresse.

Du kan også bruge følgende EXO PowerShell-kommando til at ændre den primære SMTP-adresse for en Microsoft 365-gruppe/Teams:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Eksempel:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
