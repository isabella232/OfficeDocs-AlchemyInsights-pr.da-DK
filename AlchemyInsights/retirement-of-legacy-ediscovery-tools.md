---
title: Tilbagetrækning af ældre eDiscovery-værktøjer
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
- "9001487"
- "3523"
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798543"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Tilbagetrækning af ældre eDiscovery-værktøjer

Som et resultat af den nye og forbedrede eDiscovery-funktionalitet i Microsoft 365 Compliance Center vil følgende ældre eDiscovery-værktøjer og -commandlets udgå i de kommende måneder:

- [Direkte eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) [og direkte vente hold](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) i Exchange Administration.

- Exchange Online PowerShell-cmdletter, der understøtter In-Place eDiscovery og In-Place ventepositioner. (Disse cmdlet'er identificeres samlet som *-MailboxSearch-cmdlet'er). Dette omfatter følgende cmdlet'er:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- [Cmdlet'en](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) Søgepostkasse i Exchange Online PowerShell.
- Følgende handlinger i Exchange Web Services API:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Avanceret eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Tidslinje for tilbagetrækning**:
- **1. juli 2020** Du kan ikke længere oprette nye søgninger og ventende funktioner, men du kan køre, redigere og slette eksisterende søgninger på eget ansvar. Microsoft Support understøtter ikke længere In-Place eDiscovery-& i EAC.
    
- **1. oktober 2020** In-Place eDiscovery &-ventende funktioner i EAC anbringes i skrivebeskyttet tilstand, så du kun kan fjerne eksisterende søgninger og ventefunktioner.

**Du kan finde flere oplysninger i:**

 - [Overfør ældre eDiscovery-søgninger og -ventende funktioner til Microsoft 365-overholdelsescenteret](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Tilbagetrækning af ældre eDiscovery-værktøjer](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Ofte stillede spørgsmål om In-Place eDiscovery og In-Place hold](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



