---
title: Alderspension af ældre eDiscovery-værktøjer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 2315c4c651a83f0ecc78c0171f32aba13bc93f8c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727777"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Alderspension af ældre eDiscovery-værktøjer

Som et resultat af de nye og forbedrede eDiscovery-funktioner i Microsoft 365 Compliance Center, vil følgende ældre eDiscovery-værktøjer og commandlets blive udgået i de kommende måneder:

- [Direkte eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) og [lokale ventepositioner](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) i Exchange Admin Center.

- Exchange Online PowerShell-cmdletter, der understøtter lokale eDiscovery-og lokale ventepositioner. Disse cmdletter identificeres samlet som *-MailboxSearch-cmdletter. Dette omfatter følgende cmdletter:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Cmdlet'en [Search-postkasse](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) i Exchange Online PowerShell.
- Følgende handlinger i Exchange Web Services API:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Avanceret eDiscovery v 1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Tidslinje for Pension**:
- **1. juli 2020** Du kan ikke længere oprette nye søgninger og ventepositioner, men du kan køre, redigere og slette eksisterende søgninger på din egen risiko. Microsoft Support understøtter ikke længere direkte eDiscovery-&-ventepositioner i EAC.
    
- **1. oktober 2020** Direkte eDiscovery & indeholder funktionaliteten i EAC bliver placeret i skrivebeskyttet tilstand, så du kun kan fjerne eksisterende søgninger og ventepositioner.

**Du kan finde flere oplysninger i**:

 - [Overføre ældre eDiscovery-søgninger og-ventepositioner til Microsoft 365-Overholdelsescenter](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Alderspension af ældre eDiscovery-værktøjer](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Ofte stillede spørgsmål om lokale eDiscovery-og lokale ventepositioner](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



