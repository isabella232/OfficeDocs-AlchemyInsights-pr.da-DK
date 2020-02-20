---
title: Pensionering af Ældre eDiscovery-værktøjer
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
ms.openlocfilehash: c4632b52dde579b7d5b2e6e15f1583300a0bd136
ms.sourcegitcommit: a7c17217c170ead24571421baaf5a14f1525b1a6
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/20/2020
ms.locfileid: "42157548"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Pensionering af Ældre eDiscovery-værktøjer

Som et resultat af den nye og forbedrede eDiscovery-funktionalitet i Microsoft 365 Compliance Center vil følgende ældre eDiscovery-værktøjer og -kommandoer blive trukket tilbage i de kommende måneder:

- [Indbyggede eDiscovery-](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) og [in-place-holdere](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) i Exchange Administration.

- Exchange Online PowerShell-cmdletter, der understøtter in-place eDiscovery og in-place holdere. (Disse cmdlets er kollektivt identificeret som *-MailboxSearch cmdlets.) Dette omfatter følgende cmdlets:

    - [Søgning efter ny postkasse](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Søg efter startpostkasse](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-PostkasseSøgning](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-PostkasseSøg](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- [Cmdlet'en Søgepostkasse](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) i Exchange Online PowerShell.
- Følgende handlinger i Exchange Web Services API:
    - [FåSøgbarepostkasser](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailbokse](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Avanceret eDiscovery v1.0 fra Office 365](https://docs.microsoft.com/en-us/microsoft-365/compliance/office-365-advanced-ediscovery)

**Tidslinje for pensionering**:
- 1. april 2020: Du kan ikke oprette nye søgninger og ventepositioner, men du kan stadig køre, redigere og slette eksisterende søgninger på egen risiko. Microsoft Support understøtter ikke længere In-Place eDiscovery & holder i EAC.

- 1. juli 2020: Funktionen In-Place eDiscovery & Holder i EAC placeres i skrivebeskyttet tilstand. Det betyder, at du kun kan fjerne eksisterende søgninger og tilbageholdelser.

**Yderligere oplysninger finder du i:**

 - [Overfør ældre eDiscovery-søgninger og -tilbageholdelser til Microsoft 365-overholdelsescenter](https://docs.microsoft.com/en-us/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Pensionering af ældre eDiscovery-værktøjer](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Ofte stillede spørgsmål om in-place eDiscovery og in-place holder](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



