---
title: Administrere journalisering
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004299"
- "7677"
ms.openlocfilehash: 2fcd0f386d2da8cad19fcc9872482bb75fe00dd2
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744378"
---
# <a name="manage-journaling"></a><span data-ttu-id="95d43-102">Administrere journalisering</span><span class="sxs-lookup"><span data-stu-id="95d43-102">Manage journaling</span></span>

<span data-ttu-id="95d43-103">Journalisering kan hjælpe din organisation med at overholde juridiske, lovgivningsmæssige og organisatoriske krav ved at registrere indgående og udgående mailkommunikation.</span><span class="sxs-lookup"><span data-stu-id="95d43-103">Journaling can help your organization respond to legal, regulatory, and organizational compliance requirements by recording inbound and outbound email communications.</span></span> <span data-ttu-id="95d43-104">Husk:</span><span class="sxs-lookup"><span data-stu-id="95d43-104">Keep in mind:</span></span>

* <span data-ttu-id="95d43-105">Du skal have tilladelse [til organisationsadministration](https://go.microsoft.com/fwlink/?linkid=2115259) og [datastyring,](https://go.microsoft.com/fwlink/?linkid=2115469) før du kan administrere journalisering.</span><span class="sxs-lookup"><span data-stu-id="95d43-105">You need to have [Organization Management](https://go.microsoft.com/fwlink/?linkid=2115259) and [Records Management](https://go.microsoft.com/fwlink/?linkid=2115469) permissions before you can manage journaling.</span></span>
* <span data-ttu-id="95d43-106">Du skal have en journalpostkasse og (eventuelt) en alternativ journalpostkasse konfigureret.</span><span class="sxs-lookup"><span data-stu-id="95d43-106">You need to have a journal mailbox and (optionally) an alternate journaling mailbox configured.</span></span> <span data-ttu-id="95d43-107">Hvis du vil have mere at vide, [skal du se Konfigurere journalisering i Exchange Online.](https://go.microsoft.com/fwlink/?linkid=2115260)</span><span class="sxs-lookup"><span data-stu-id="95d43-107">To learn more, see [Configure Journaling in Exchange Online](https://go.microsoft.com/fwlink/?linkid=2115260).</span></span>
* <span data-ttu-id="95d43-108">I Exchange Online er der en grænse for antallet af journalregler, du kan oprette.</span><span class="sxs-lookup"><span data-stu-id="95d43-108">In Exchange Online, there's a limit to the number of journal rules that you can create.</span></span> <span data-ttu-id="95d43-109">Du kan finde flere oplysninger [i Journal, transport- og indbakkeregelbegrænsninger.](https://go.microsoft.com/fwlink/?linkid=2115261)</span><span class="sxs-lookup"><span data-stu-id="95d43-109">For details, see [Journal, transport, and inbox rule limits](https://go.microsoft.com/fwlink/?linkid=2115261).</span></span>
* <span data-ttu-id="95d43-110">Exchange Online understøtter ikke levering af journalrapporter til en Exchange Online-postkasse.</span><span class="sxs-lookup"><span data-stu-id="95d43-110">Exchange Online doesn't support delivering journal reports to an Exchange Online mailbox.</span></span> <span data-ttu-id="95d43-111">Du skal angive mailadressen på et lokalt arkiveringssystem eller en tredjeparts arkiveringstjeneste som journalpostkasse.</span><span class="sxs-lookup"><span data-stu-id="95d43-111">You must specify the email address of an on-premises archiving system or a third-party archiving service as the journaling mailbox.</span></span>
