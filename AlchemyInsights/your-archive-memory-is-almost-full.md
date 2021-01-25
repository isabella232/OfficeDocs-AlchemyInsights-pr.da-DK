---
title: Din Arkiv postkasse er næsten fuld
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
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974275"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Din Arkiv postkasse er næsten fuld

Hvis brugeren modtager advarslen. **Din postkasse er næsten fuld**, eller du har brug for at øge størrelsen på postkassen i deres arkiv, da her er nogle tip:

1. Hvis brugeren er tildelt en Exchange Online-plan 1, skal du opgradere til **Exchange Online plan 2** -licens for at øge størrelsen fra 50 GB til 100 GB.
1. Hvis brugeren allerede er tildelt en af følgende: **Exchange Online plan 2** eller en Exchange Online-plan 1 med et tilføjelsesprogram til Exchange Online-arkivering, skal du følge nedenstående trin for at aktivere automatisk udvidelse af arkivering:.
 
    1. [Opret forbindelse til Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    2. Kør følgende Group for brugeren:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Kør følgende Group for at bekræfte, at den er aktiveret for brugeren:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Du kan finde flere oplysninger under:

- [ Aktivér ubegrænset arkivering – hjælp til administratorer-Microsoft 365-kompatibilitet | Microsoft-dokumenter](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Online-begrænsninger – service beskrivelser | Microsoft-dokumenter](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Opgrader til en anden virksomhedsplan | Microsoft-dokumenter](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

