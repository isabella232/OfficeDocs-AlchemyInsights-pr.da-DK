---
title: Kalendertilladelser
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862059"
---
# <a name="calendar-permissions"></a>Kalendertilladelser

Brugerne kan ændre deres egne kalendertilladelser med Outlook på internettet eller andre klienter, men som administrator skal du muligvis også undersøge det.  
Med Exchange PowerShell-cmdlet får du tilladelse til at følge en brugers kalender:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Hvis du vil se flere oplysninger, skal du se følgende:

- [Hent-PostkasseFoldErPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Tilføj postkassefoldErPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Kalendertilladelser bruges i deling af kalendere for at få vist flere oplysninger om deling af en Outlook-kalender i disse artikler:

- [Del en Outlook-kalender med andre personer](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Dele din kalender i Outlook på internettet til virksomheder](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Hvis du vil foretage fejlfinding af kalendertilladelse, kan du bruge værktøjet [Support og Genoprettelsesassistent.](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f)