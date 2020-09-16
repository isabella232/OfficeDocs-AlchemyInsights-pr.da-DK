---
title: 1336 RecoverableItems-mappen er fuld
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741261"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="99d3b-102">Mappen Genoprettelige elementer er fuld</span><span class="sxs-lookup"><span data-stu-id="99d3b-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="99d3b-103">For Exchange Online-postkasser er standardlager grænsen for mappen Genoprettelige elementer 30 GB.</span><span class="sxs-lookup"><span data-stu-id="99d3b-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="99d3b-104">Lagergrænsen for mappen Genoprettelige elementer øges automatisk til 100 GB, hvis postkassen er placeret i retssag, eDiscovery-venteposition eller er tildelt en opbevaringspolitik.</span><span class="sxs-lookup"><span data-stu-id="99d3b-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="99d3b-105">Når mappen Genoprettelige elementer Når lagergrænsen, påvirkes postkasse funktionaliteten på følgende måder:</span><span class="sxs-lookup"><span data-stu-id="99d3b-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="99d3b-106">Brugeren kan ikke slette elementer fra postkassen.</span><span class="sxs-lookup"><span data-stu-id="99d3b-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="99d3b-107">Assistent til administrerede mapper kan ikke slette elementer, der er baseret på opbevarings kode eller indstillinger for administrerede mapper.</span><span class="sxs-lookup"><span data-stu-id="99d3b-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="99d3b-108">For postkasser, hvor en enkelt element gendannelse er aktiveret eller er sat i venteposition, kan der ikke gemmes versioner af de elementer, der er blevet redigeret af brugeren.</span><span class="sxs-lookup"><span data-stu-id="99d3b-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="99d3b-109">For postkasser, hvor logføring for postkasse overvågning er aktiveret, kan der ikke gemmes nogen poster til overvågningslogfiler for postkassen i under mappen reitems i Genoprettelige elementer.</span><span class="sxs-lookup"><span data-stu-id="99d3b-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="99d3b-110">For postkasser, der ikke er i venteposition, kan administratorer bruge `Search-Mailbox -SearchDumpsterOnly -DeleteContent` kommandoen i Exchange Online PowerShell til at slette elementer i mappen Genoprettelige elementer.</span><span class="sxs-lookup"><span data-stu-id="99d3b-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="99d3b-111">Hvis du vil have mere at vide, skal du se følgende emner:</span><span class="sxs-lookup"><span data-stu-id="99d3b-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="99d3b-112">Søg efter og slet meddelelser</span><span class="sxs-lookup"><span data-stu-id="99d3b-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="99d3b-113">Søg-postkasse</span><span class="sxs-lookup"><span data-stu-id="99d3b-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="99d3b-114">For postkasser, der er i venteposition, skal administratorer fjerne ventepositionen, før de kan slette elementer fra mappen Genoprettelige elementer.</span><span class="sxs-lookup"><span data-stu-id="99d3b-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="99d3b-115">Hvis du vil have mere at vide, skal du se [Slet elementer i mappen Genoprettelige elementer i skybaserede postkasser i venteposition](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="99d3b-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="99d3b-116">For at forhindre, at mappen Genoprettelige elementer bliver fuld, kan administratorer øge lagergrænsen for mappen Genoprettelige elementer for postkasser i venteposition og konfigurere en opbevaringspolitik for postkasser, der flytter elementer fra mappen Genoprettelige elementer til brugerens Arkiv postkasse.</span><span class="sxs-lookup"><span data-stu-id="99d3b-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="99d3b-117">Se [Forøg kvoten for Genoprettelige elementer for postkasser i venteposition](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="99d3b-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
