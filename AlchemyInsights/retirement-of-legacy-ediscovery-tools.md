---
title: Alderspension af ældre eDiscovery-værktøjer
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
ms.openlocfilehash: 94cd2127240be5faacd397ba6255fdb16e364308
ms.sourcegitcommit: d4fc2a03af69e28e96075812d040fdd34d2e23f0
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/26/2020
ms.locfileid: "46902614"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="50f96-102">Alderspension af ældre eDiscovery-værktøjer</span><span class="sxs-lookup"><span data-stu-id="50f96-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="50f96-103">Som et resultat af de nye og forbedrede eDiscovery-funktioner i Microsoft 365 Compliance Center, vil følgende ældre eDiscovery-værktøjer og commandlets blive udgået i de kommende måneder:</span><span class="sxs-lookup"><span data-stu-id="50f96-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="50f96-104">[Direkte eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) og [lokale ventepositioner](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) i Exchange Admin Center.</span><span class="sxs-lookup"><span data-stu-id="50f96-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="50f96-105">Exchange Online PowerShell-cmdletter, der understøtter lokale eDiscovery-og lokale ventepositioner.</span><span class="sxs-lookup"><span data-stu-id="50f96-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="50f96-106">Disse cmdletter identificeres samlet som \*-MailboxSearch-cmdletter. Dette omfatter følgende cmdletter:</span><span class="sxs-lookup"><span data-stu-id="50f96-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="50f96-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="50f96-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="50f96-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="50f96-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="50f96-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="50f96-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="50f96-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="50f96-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="50f96-111">Cmdlet'en [Search-postkasse](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) i Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="50f96-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="50f96-112">Følgende handlinger i Exchange Web Services API:</span><span class="sxs-lookup"><span data-stu-id="50f96-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="50f96-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="50f96-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="50f96-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="50f96-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="50f96-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="50f96-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="50f96-116">Avanceret eDiscovery v 1.0</span><span class="sxs-lookup"><span data-stu-id="50f96-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="50f96-117">**Tidslinje for Pension**:</span><span class="sxs-lookup"><span data-stu-id="50f96-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="50f96-118">**1. juli 2020** Du kan ikke længere oprette nye søgninger og ventepositioner, men du kan køre, redigere og slette eksisterende søgninger på din egen risiko.</span><span class="sxs-lookup"><span data-stu-id="50f96-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="50f96-119">Microsoft Support understøtter ikke længere direkte eDiscovery-&-ventepositioner i EAC.</span><span class="sxs-lookup"><span data-stu-id="50f96-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="50f96-120">**1. oktober 2020** Direkte eDiscovery & indeholder funktionaliteten i EAC bliver placeret i skrivebeskyttet tilstand, så du kun kan fjerne eksisterende søgninger og ventepositioner.</span><span class="sxs-lookup"><span data-stu-id="50f96-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="50f96-121">**Du kan finde flere oplysninger i**:</span><span class="sxs-lookup"><span data-stu-id="50f96-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="50f96-122">Overføre ældre eDiscovery-søgninger og-ventepositioner til Microsoft 365-Overholdelsescenter</span><span class="sxs-lookup"><span data-stu-id="50f96-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="50f96-123">Alderspension af ældre eDiscovery-værktøjer</span><span class="sxs-lookup"><span data-stu-id="50f96-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="50f96-124">Ofte stillede spørgsmål om lokale eDiscovery-og lokale ventepositioner</span><span class="sxs-lookup"><span data-stu-id="50f96-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



