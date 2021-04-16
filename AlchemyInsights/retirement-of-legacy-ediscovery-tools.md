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
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="ee77e-102">Tilbagetrækning af ældre eDiscovery-værktøjer</span><span class="sxs-lookup"><span data-stu-id="ee77e-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="ee77e-103">Som et resultat af den nye og forbedrede eDiscovery-funktionalitet i Microsoft 365 Compliance Center vil følgende ældre eDiscovery-værktøjer og -commandlets udgå i de kommende måneder:</span><span class="sxs-lookup"><span data-stu-id="ee77e-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="ee77e-104">[Direkte eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) [og direkte vente hold](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) i Exchange Administration.</span><span class="sxs-lookup"><span data-stu-id="ee77e-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="ee77e-105">Exchange Online PowerShell-cmdletter, der understøtter In-Place eDiscovery og In-Place ventepositioner.</span><span class="sxs-lookup"><span data-stu-id="ee77e-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="ee77e-106">(Disse cmdlet'er identificeres samlet som \*-MailboxSearch-cmdlet'er). Dette omfatter følgende cmdlet'er:</span><span class="sxs-lookup"><span data-stu-id="ee77e-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="ee77e-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="ee77e-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="ee77e-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="ee77e-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="ee77e-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="ee77e-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="ee77e-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="ee77e-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="ee77e-111">[Cmdlet'en](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) Søgepostkasse i Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ee77e-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="ee77e-112">Følgende handlinger i Exchange Web Services API:</span><span class="sxs-lookup"><span data-stu-id="ee77e-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="ee77e-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="ee77e-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="ee77e-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="ee77e-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="ee77e-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="ee77e-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="ee77e-116">Avanceret eDiscovery v1.0</span><span class="sxs-lookup"><span data-stu-id="ee77e-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="ee77e-117">**Tidslinje for tilbagetrækning**:</span><span class="sxs-lookup"><span data-stu-id="ee77e-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="ee77e-118">**1. juli 2020** Du kan ikke længere oprette nye søgninger og ventende funktioner, men du kan køre, redigere og slette eksisterende søgninger på eget ansvar.</span><span class="sxs-lookup"><span data-stu-id="ee77e-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="ee77e-119">Microsoft Support understøtter ikke længere In-Place eDiscovery-& i EAC.</span><span class="sxs-lookup"><span data-stu-id="ee77e-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="ee77e-120">**1. oktober 2020** In-Place eDiscovery &-ventende funktioner i EAC anbringes i skrivebeskyttet tilstand, så du kun kan fjerne eksisterende søgninger og ventefunktioner.</span><span class="sxs-lookup"><span data-stu-id="ee77e-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="ee77e-121">**Du kan finde flere oplysninger i:**</span><span class="sxs-lookup"><span data-stu-id="ee77e-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="ee77e-122">Overfør ældre eDiscovery-søgninger og -ventende funktioner til Microsoft 365-overholdelsescenteret</span><span class="sxs-lookup"><span data-stu-id="ee77e-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="ee77e-123">Tilbagetrækning af ældre eDiscovery-værktøjer</span><span class="sxs-lookup"><span data-stu-id="ee77e-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="ee77e-124">Ofte stillede spørgsmål om In-Place eDiscovery og In-Place hold</span><span class="sxs-lookup"><span data-stu-id="ee77e-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



