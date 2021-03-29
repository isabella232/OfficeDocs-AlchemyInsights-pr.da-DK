---
title: Kontrollér, om adresser på postkasser videresendes
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 3abd45230360c61ecb62e4b7a39d1b0b547271fc
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403305"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="e820a-102">Kontrollér, om adresser på postkasser videresendes</span><span class="sxs-lookup"><span data-stu-id="e820a-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="e820a-103">Nogle gange videresender hackere brugernes mails til sig selv, så vi kontrollerer først for videresendelse af adresser og regler for postkassen.</span><span class="sxs-lookup"><span data-stu-id="e820a-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="e820a-104">Derefter kontrollerer vi overvågningslogfilerne.</span><span class="sxs-lookup"><span data-stu-id="e820a-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="e820a-105">Sådan søger du efter videresendelsesadresser:</span><span class="sxs-lookup"><span data-stu-id="e820a-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="e820a-106">Vælg   >  **Brugere, der er aktive brugere.**</span><span class="sxs-lookup"><span data-stu-id="e820a-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="e820a-107">Vælg den bruger, hvis konto er blevet kompromitteret.</span><span class="sxs-lookup"><span data-stu-id="e820a-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="e820a-108">Udvid Indstillinger for mail i **pop** op-menuen, der vises, og klik derefter **på Rediger** til **videresendelse af mail.**</span><span class="sxs-lookup"><span data-stu-id="e820a-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="e820a-109">Fjern eventuelle videresendelsesadresser, du ikke genkender.</span><span class="sxs-lookup"><span data-stu-id="e820a-109">Remove any forwarding addresses you don't recognize.</span></span>