---
title: Aktivere postkasserevision
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: aa0ff925ae891d28e31394ec66eb17c2d9710008
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429352"
---
# <a name="turn-on-mailbox-auditing"></a>Aktivere postkasserevision

Hvis du vil aktivere postkasseovervågning for en enkelt bruger eller en hel organisation, skal du køre følgende cmdlet'er fra Remote PowerShell:

- **Enkelt bruger:** Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true
- **Organisation:** Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled-$true

Du kan få mere at vide under [Administrer postkasserevision.](https://go.microsoft.com/fwlink/?linkid=2103668)