---
title: 1336 Mappen RecoverableItems er fuld
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 4f0cba480fcc05114abd8f370b84e9a37e5f2804
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510746"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="a14aa-102">Mappen Genopretteligt elementer er fuld</span><span class="sxs-lookup"><span data-stu-id="a14aa-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="a14aa-103">For Exchange Online-postkasser er standardlagergrænsen for mappen Genoprettelige elementer 30 GB.</span><span class="sxs-lookup"><span data-stu-id="a14aa-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="a14aa-104">Lagergrænsen for mappen Genoprettelige elementer øges automatisk til 100 GB, hvis postkassen placeres i Retslig tilbageholdelse, eDiscovery-venteposition eller er tildelt til en opbevaringspolitik.</span><span class="sxs-lookup"><span data-stu-id="a14aa-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="a14aa-105">Når mappen Genoprettelige elementer når lagergrænsen, påvirkes postkassefunktionaliteten på følgende måder:</span><span class="sxs-lookup"><span data-stu-id="a14aa-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="a14aa-106">Brugeren kan ikke slette elementer fra postkassen.</span><span class="sxs-lookup"><span data-stu-id="a14aa-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="a14aa-107">Assistenten for administrerede mapper kan ikke slette elementer baseret på indstillinger for opbevaringskode eller administrerede mapper.</span><span class="sxs-lookup"><span data-stu-id="a14aa-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="a14aa-108">For postkasser, hvor gendannelse af enkeltelement er aktiveret eller er sat i venteposition, kan sidebeskyttelsesprocessen for copy-on-write ikke vedligeholde versioner af elementer, der er redigeret af brugeren.</span><span class="sxs-lookup"><span data-stu-id="a14aa-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="a14aa-109">For postkasser, hvor postkasseovervågningslogføring er aktiveret, kan der ikke gemmes poster i undermappen Overvågning i undermappen Overvågning i mappen Genoprettelige elementer.</span><span class="sxs-lookup"><span data-stu-id="a14aa-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="a14aa-110">I forbindelse med postkasser, der ikke er i venteposition, kan administratorer bruge `Search-Mailbox -SearchDumpsterOnly -DeleteContent` kommandoen i Exchange Online PowerShell til at slette elementer i mappen Genoprettelige elementer.</span><span class="sxs-lookup"><span data-stu-id="a14aa-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="a14aa-111">Yderligere oplysninger finder du i følgende emner:</span><span class="sxs-lookup"><span data-stu-id="a14aa-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="a14aa-112">Søge efter og slette meddelelser</span><span class="sxs-lookup"><span data-stu-id="a14aa-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="a14aa-113">Søg-postkasse</span><span class="sxs-lookup"><span data-stu-id="a14aa-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="a14aa-114">I forbindelse med postkasser, der er i venteposition, skal administratorer fjerne ventepositionen, før de kan slette elementer fra mappen Genoprettelige elementer.</span><span class="sxs-lookup"><span data-stu-id="a14aa-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="a14aa-115">Du kan finde flere oplysninger [under Slette elementer i mappen Genoprettelige elementer i skybaserede postkasser i venteposition](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="a14aa-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="a14aa-116">Administratorer kan øge lagergrænsen for mappen Genoprettelige elementer for postkasser, der er i venteposition, og oprette en politik for opbevaring af postkasser, der flytter elementer fra mappen Genoprettelige elementer til brugerens arkivpostkasse.</span><span class="sxs-lookup"><span data-stu-id="a14aa-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="a14aa-117">Se [Øge kvoten for elementer, der kan gendannes, for postkasser i venteposition](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="a14aa-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
