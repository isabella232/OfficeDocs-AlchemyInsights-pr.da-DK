---
title: Arkivpostkassen er næsten fuld
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 085d9b211d5a8e9a0e1eb12af14d87a4e59c844a3afa012095dfd60db316ad14
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046746"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Arkivpostkassen er næsten fuld

Hvis brugeren modtager advarslen; **Din arkivpostkasse er næsten fuld**, eller du har brug for at øge størrelsen på deres arkivpostkasse. Her er nogle tip:

1. Hvis brugeren er tildelt en Exchange Online Plan 1, skal du opgradere **til Exchange Online Plan 2-licens** for at øge størrelsen fra 50 GB til 100 GB.
1. Hvis brugeren allerede er tildelt et af følgende: **Exchange Online Plan 2** eller en Exchange Online Plan 1 med et tilføjelsesprogrammet Exchange Online-arkivering, skal du følge trinnene nedenfor for at aktivere automatisk arkivering:
 
    1. [Forbind til Exchange Online Powershell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)
    2. Kør følgende kommandolet for brugeren:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Kør følgende kommandolet for at bekræfte, at den er aktiveret for brugeren:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Du kan finde flere oplysninger under:

- [Aktivér ubegrænset arkivering – Hjælp til administratorer – Microsoft 365 overholdelse | Microsoft Docs](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Online – Tjenestebeskrivelser | Microsoft Docs](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Opgrader til en anden | Microsoft Docs](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

