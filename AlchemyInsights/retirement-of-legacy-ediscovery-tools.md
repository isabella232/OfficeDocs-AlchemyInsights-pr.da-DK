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
ms.openlocfilehash: af9a0bd8ff4294575ac68f37d4997bb50b132ce7
ms.sourcegitcommit: 9ab422063e5a474c92ed956d42d222b90336fecb
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/11/2020
ms.locfileid: "42600357"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="64a2c-102">Pensionering af ældre eDiscovery-værktøjer</span><span class="sxs-lookup"><span data-stu-id="64a2c-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="64a2c-103">Som et resultat af den nye og forbedrede eDiscovery-funktionalitet i Microsoft 365 Compliance Center vil følgende ældre eDiscovery-værktøjer og -kommandoer blive trukket tilbage i de kommende måneder:</span><span class="sxs-lookup"><span data-stu-id="64a2c-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="64a2c-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) [og in-place Holds i](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) Exchange Administration.</span><span class="sxs-lookup"><span data-stu-id="64a2c-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="64a2c-105">Exchange Online PowerShell-cmdletterne, der understøtter eDiscovery og in-place-hold.</span><span class="sxs-lookup"><span data-stu-id="64a2c-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="64a2c-106">(Disse cmdletter identificeres samlet som \*-MailboxSearch-cmdletter). Dette omfatter følgende cmdletter:</span><span class="sxs-lookup"><span data-stu-id="64a2c-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="64a2c-107">Søg efter ny postkasse</span><span class="sxs-lookup"><span data-stu-id="64a2c-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="64a2c-108">Start-postkasseSøgning</span><span class="sxs-lookup"><span data-stu-id="64a2c-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="64a2c-109">Stop-PostkasseSøg</span><span class="sxs-lookup"><span data-stu-id="64a2c-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="64a2c-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="64a2c-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="64a2c-111">[Søgepostkassen](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet i Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="64a2c-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="64a2c-112">Følgende handlinger i Exchange Web Services API:</span><span class="sxs-lookup"><span data-stu-id="64a2c-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="64a2c-113">GetSearchablePostkasser</span><span class="sxs-lookup"><span data-stu-id="64a2c-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="64a2c-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="64a2c-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="64a2c-115">Hent HoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="64a2c-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="64a2c-116">Avanceret EDiscovery v1.0 i Office 365</span><span class="sxs-lookup"><span data-stu-id="64a2c-116">Office 365 Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="64a2c-117">**Tidslinje for pensionering**:</span><span class="sxs-lookup"><span data-stu-id="64a2c-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="64a2c-118">1. april 2020: Du kan ikke oprette nye søgninger og tilbageholdelser, men du kan stadig køre, redigere og slette eksisterende søgninger på egen risiko.</span><span class="sxs-lookup"><span data-stu-id="64a2c-118">April 1, 2020: You won't be able to create new searches and holds, but you can still run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="64a2c-119">Microsoft Support understøtter ikke længere direkte eDiscovery-&-ventepositioner i EAC.</span><span class="sxs-lookup"><span data-stu-id="64a2c-119">Microsoft Support will no longer support In-Place eDiscovery & Holds in the EAC.</span></span>

- <span data-ttu-id="64a2c-120">1. juli 2020: Den indbyggede eDiscovery-&-funktioner i EAC placeres i skrivebeskyttet tilstand.</span><span class="sxs-lookup"><span data-stu-id="64a2c-120">July 1, 2020: The In-Place eDiscovery & Holds functionality in the EAC will be placed in a read-only mode.</span></span> <span data-ttu-id="64a2c-121">Det betyder, at du kun kan fjerne eksisterende søgninger og tilbageholdelser.</span><span class="sxs-lookup"><span data-stu-id="64a2c-121">This means you'll only be able to remove existing searches and holds.</span></span>

<span data-ttu-id="64a2c-122">**Yderligere oplysninger finder du i**:</span><span class="sxs-lookup"><span data-stu-id="64a2c-122">**For more information, see**:</span></span>

 - [<span data-ttu-id="64a2c-123">Overfør ældre eDiscovery-søgninger og -tilbageholdelser til Microsoft 365-kompatibilitetscenter</span><span class="sxs-lookup"><span data-stu-id="64a2c-123">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="64a2c-124">Pensionering af ældre eDiscovery-værktøjer</span><span class="sxs-lookup"><span data-stu-id="64a2c-124">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="64a2c-125">Ofte stillede spørgsmål om in-place eDiscovery og in-place holds</span><span class="sxs-lookup"><span data-stu-id="64a2c-125">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



