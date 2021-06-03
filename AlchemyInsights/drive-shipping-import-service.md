---
title: Drevforsendelse i Microsoft 365 Importtjeneste
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11514"
- "9003046"
ms.openlocfilehash: 85d6e723e56b01fd9914165d8c9740f3b055947d
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731440"
---
# <a name="drive-shipping-in-the-microsoft-365-import-service"></a><span data-ttu-id="b19fe-102">Drevforsendelse i Microsoft 365 Importtjeneste</span><span class="sxs-lookup"><span data-stu-id="b19fe-102">Drive shipping in the Microsoft 365 Import Service</span></span>

<span data-ttu-id="b19fe-103">Brug drevforsendelse ved at kopiere PST'er til en harddisk og derefter sende harddisken til Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b19fe-103">Use Drive shipping by copying PSTs to a hard drive and then shipping the hard drive to Microsoft.</span></span>

<span data-ttu-id="b19fe-104">Sådan startes jobbet:</span><span class="sxs-lookup"><span data-stu-id="b19fe-104">To start the job:</span></span>

1. <span data-ttu-id="b19fe-105">Vælg Importér Microsoft 365 i Center **for** overholdelse af regler og standarder under **Styring af oplysninger.**</span><span class="sxs-lookup"><span data-stu-id="b19fe-105">In the Microsoft 365 Compliance Center under **Information Governance**, select **Import**.</span></span>

1. <span data-ttu-id="b19fe-106">Vælg **Vælg importjobtype**, og vælg derefter **Næste**.</span><span class="sxs-lookup"><span data-stu-id="b19fe-106">Select **Choose import job type**, and then select **Next**.</span></span>

1. <span data-ttu-id="b19fe-107">Hvis du vil se trinnene for denne importindstilling, skal **du vælge Send harddiske til en af vores fysiske placeringer.**</span><span class="sxs-lookup"><span data-stu-id="b19fe-107">To see the steps for this import option, select **Ship hard drives to one of our physical locations**.</span></span>

<span data-ttu-id="b19fe-108">Her er nogle ting, du skal huske:</span><span class="sxs-lookup"><span data-stu-id="b19fe-108">Here are some things to remember:</span></span>

- <span data-ttu-id="b19fe-109">Du skal have tildelt rollen Postkasse Import Eksport i en Exchange Online for at importere PST-filer Microsoft 365 postkasser.</span><span class="sxs-lookup"><span data-stu-id="b19fe-109">You must be assigned the Mailbox Import Export role in Exchange Online to import PST files to Microsoft 365 mailboxes.</span></span>
<span data-ttu-id="b19fe-110">Ydeevnen kan påvirkes for PST'er, der er større end 20 GB.</span><span class="sxs-lookup"><span data-stu-id="b19fe-110">Performance might be impacted for PSTs larger than 20GB.</span></span>

- <span data-ttu-id="b19fe-111">Kun 2,5"-solid state-drev (SSD'er) eller 2,5" eller 3,5" SATA II/III-interne harddiske understøttes.</span><span class="sxs-lookup"><span data-stu-id="b19fe-111">Only 2.5-inch solid-state drives (SSDs) or 2.5-inch or 3.5-inch SATA II/III internal hard drives are supported.</span></span>
<span data-ttu-id="b19fe-112">Harddisk, der indeholder PST-filer, skal være krypteret BitLocker.</span><span class="sxs-lookup"><span data-stu-id="b19fe-112">Hard drive containing PST files must be encrypted with BitLocker.</span></span>

- <span data-ttu-id="b19fe-113">Import af PST-filer til postkasser Microsoft 365 drevforsendelse koster 2 USD pr. GB data.</span><span class="sxs-lookup"><span data-stu-id="b19fe-113">The cost to import PST files to Microsoft 365 mailboxes using drive shipping is $2 USD per GB of data.</span></span>

<span data-ttu-id="b19fe-114">Du kan finde flere oplysninger om brug af drevforsendelsesmetode til import af PST'er i Brug drevforsendelse til at importere [din organisations PST-filer.](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365)</span><span class="sxs-lookup"><span data-stu-id="b19fe-114">For additional information on using the Drive shipping method for importing PSTs, see [Use drive shipping to import your organization's PST files](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365).</span></span>