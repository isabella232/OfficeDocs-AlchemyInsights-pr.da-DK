---
title: Kalendertilladelser
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: bbd49134bd4a4451649b76bb5f60b19065910cae
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819902"
---
# <a name="calendar-permissions"></a>Kalendertilladelser

Brugere kan ændre deres egne kalendertilladelser med Outlook på internettet eller andre klienter, men som administrator kan det også være nødvendigt at undersøge det.  
Med Exchange PowerShell-cmdlet'en får du vist tilladelsen til en brugers kalender:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Hvis du vil se flere oplysninger, skal du se følgende:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Tilføjelsespostkassemappe](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Kalendertilladelser bruges i deling af kalendere, for at se flere oplysninger om deling af en Outlook-kalender, skal du se følgende artikler:

- [Del en Outlook-kalender med andre personer](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Del din kalender i Outlook på internettet til virksomheder](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Hvis du vil foretage fejlfinding i forbindelse med kalendertilladelser, kan [du bruge værktøjet Support- og genoprettelsesassistent.](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f)