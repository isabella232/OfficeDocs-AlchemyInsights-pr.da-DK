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
# <a name="turn-on-mailbox-auditing"></a><span data-ttu-id="fee3e-102">Aktivere postkasserevision</span><span class="sxs-lookup"><span data-stu-id="fee3e-102">Turn on mailbox auditing</span></span>

<span data-ttu-id="fee3e-103">Hvis du vil aktivere postkasseovervågning for en enkelt bruger eller en hel organisation, skal du køre følgende cmdlet'er fra Remote PowerShell:</span><span class="sxs-lookup"><span data-stu-id="fee3e-103">To turn on mailbox auditing for a single user or an entire organization, run the following cmdlets from Remote PowerShell:</span></span>

- <span data-ttu-id="fee3e-104">**Enkelt bruger:** Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="fee3e-104">**Single user**: Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
- <span data-ttu-id="fee3e-105">**Organisation:** Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled-$true</span><span class="sxs-lookup"><span data-stu-id="fee3e-105">**Organization**: Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>

<span data-ttu-id="fee3e-106">Du kan få mere at vide under [Administrer postkasserevision.](https://go.microsoft.com/fwlink/?linkid=2103668)</span><span class="sxs-lookup"><span data-stu-id="fee3e-106">To learn more, see [Manage mailbox auditing](https://go.microsoft.com/fwlink/?linkid=2103668).</span></span>