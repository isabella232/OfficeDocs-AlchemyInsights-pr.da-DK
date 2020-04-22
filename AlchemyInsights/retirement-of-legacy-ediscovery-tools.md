---
title: Pensionering af ældre eDiscovery-værktøjer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 262cca0feee17d1f929a5a94a4dd6c1ec317f6ec
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/21/2020
ms.locfileid: "43650562"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Pensionering af ældre eDiscovery-værktøjer

Som et resultat af den nye og forbedrede eDiscovery-funktionalitet i Microsoft 365 Compliance Center vil følgende ældre eDiscovery-værktøjer og -kommandoer blive trukket tilbage i de kommende måneder:

- [In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) [og in-place Holds i](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) Exchange Administration.

- Exchange Online PowerShell-cmdletterne, der understøtter eDiscovery og in-place-hold. (Disse cmdletter identificeres samlet som *-MailboxSearch-cmdletter). Dette omfatter følgende cmdletter:

    - [Søg efter ny postkasse](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-postkasseSøgning](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-PostkasseSøg](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- [Søgepostkassen](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet i Exchange Online PowerShell.
- Følgende handlinger i Exchange Web Services API:
    - [GetSearchablePostkasser](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [Hent HoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Avanceret eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Tidslinje for pensionering**:
- 1. april 2020: Du kan ikke oprette nye søgninger og tilbageholdelser, men du kan stadig køre, redigere og slette eksisterende søgninger på egen risiko. Microsoft Support understøtter ikke længere direkte eDiscovery-&-ventepositioner i EAC.

- 1. juli 2020: Den indbyggede eDiscovery-&-funktioner i EAC placeres i skrivebeskyttet tilstand. Det betyder, at du kun kan fjerne eksisterende søgninger og tilbageholdelser.

**Yderligere oplysninger finder du i**:

 - [Overfør ældre eDiscovery-søgninger og -tilbageholdelser til Microsoft 365-kompatibilitetscenter](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Pensionering af ældre eDiscovery-værktøjer](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Ofte stillede spørgsmål om in-place eDiscovery og in-place holds](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



