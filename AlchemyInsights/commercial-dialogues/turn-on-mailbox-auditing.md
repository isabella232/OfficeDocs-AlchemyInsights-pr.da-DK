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
ms.openlocfilehash: 797dd57aaa43e879c015a36c79c8c9fb13e04ae894b33b0f7c6d9694d1ae1960
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058032"
---
# <a name="turn-on-mailbox-auditing"></a>Aktivere postkasserevision

Hvis du vil aktivere postkasseovervågning for en enkelt bruger eller en hel organisation, skal du køre følgende cmdlet'er fra Remote PowerShell:

- **Enkelt bruger:** Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true
- **Organisation:** Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true

Du kan få mere at vide [under Administrer postkasse overvågning](https://go.microsoft.com/fwlink/?linkid=2103668).