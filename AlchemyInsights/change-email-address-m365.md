---
title: Skift mailadressen for en Microsoft 365-gruppe eller Microsoft Teams
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
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756551"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Skift mailadressen for en Microsoft 365-gruppe eller Microsoft Teams

Du kan ændre mailadressen for en Microsoft 365-gruppe eller Microsoft Teams ved at bruge [Microsoft 365 Administration](https://admin.microsoft.com/). Markér blot gruppen, og vælg @rediger mailadresse.

Du kan også bruge følgende EXO PowerShell-kommando til at ændre den primære SMTP-adresse for en Microsoft 365-gruppe/Teams:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Eksempel:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
