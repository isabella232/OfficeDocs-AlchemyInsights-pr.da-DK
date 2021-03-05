---
title: Kontrollér, om adresser på postkasser videresendes
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 17/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 1b0a6c8fe368196f2d1f9811aea895c2c024b2e6
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481804"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="e7eb4-102">Kontrollér, om adresser på postkasser videresendes</span><span class="sxs-lookup"><span data-stu-id="e7eb4-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="e7eb4-103">Nogle gange kan hackere videresende brugernes mails til sig selv, så vi kontrollerer først for videresendelsesadresser og regler for postkassen.</span><span class="sxs-lookup"><span data-stu-id="e7eb4-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="e7eb4-104">Derefter kontrollerer vi overvågningslogfilerne.</span><span class="sxs-lookup"><span data-stu-id="e7eb4-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="e7eb4-105">Sådan søger du efter videresendelsesadresser:</span><span class="sxs-lookup"><span data-stu-id="e7eb4-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="e7eb4-106">Vælg   >  **Brugere, der er aktive brugere.**</span><span class="sxs-lookup"><span data-stu-id="e7eb4-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="e7eb4-107">Vælg den bruger, hvis konto er blevet kompromitteret.</span><span class="sxs-lookup"><span data-stu-id="e7eb4-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="e7eb4-108">Udvid Indstillinger for mail i **pop** op-menuen, der vises, og klik derefter **på Rediger** til **videresendelse af mail.**</span><span class="sxs-lookup"><span data-stu-id="e7eb4-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="e7eb4-109">Fjern eventuelle videresendelsesadresser, du ikke kan genkende.</span><span class="sxs-lookup"><span data-stu-id="e7eb4-109">Remove any forwarding addresses you don't recognize.</span></span>