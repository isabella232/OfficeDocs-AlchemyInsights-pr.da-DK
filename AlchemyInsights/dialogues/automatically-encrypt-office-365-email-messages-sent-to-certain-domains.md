---
title: Kryptere Office 365-mails, der sendes til bestemte domæner, automatisk
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524003"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a><span data-ttu-id="d1ecc-102">Kryptere Office 365-mails, der sendes til bestemte domæner, automatisk</span><span class="sxs-lookup"><span data-stu-id="d1ecc-102">Automatically encrypt Office 365 email messages sent to certain domains</span></span>

1. <span data-ttu-id="d1ecc-103">I [Exchange Administration skal du](https://outlook.office365.com/ecp/)vælge **mailflow > regler.**</span><span class="sxs-lookup"><span data-stu-id="d1ecc-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="d1ecc-104">Klik på **ikonet Nyt (+),** og klik derefter på **Anvend Office 365-meddelelseskryptering og rettighedsbeskyttelse på meddelelser.**</span><span class="sxs-lookup"><span data-stu-id="d1ecc-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="d1ecc-105">Skriv **et navn** til reglen under Navn, f.eks. Kryptér *meddelelser, der sendes contoso.com.*</span><span class="sxs-lookup"><span data-stu-id="d1ecc-105">In **Name**, enter a name for the rule, such as *Encrypt messages sent to contoso.com*.</span></span>
4. <span data-ttu-id="d1ecc-106">I **Anvend denne regel, hvis,** skal **du vælge > domænet er.**</span><span class="sxs-lookup"><span data-stu-id="d1ecc-106">In **Apply this rule if**, choose **The recipient > domain is**.</span></span> 
5. <span data-ttu-id="d1ecc-107">Angiv navnet på domænet, f.eks. **contoso.com.**</span><span class="sxs-lookup"><span data-stu-id="d1ecc-107">Enter the name of the domain, such as **contoso.com**.</span></span>
6. <span data-ttu-id="d1ecc-108">Klik på **ikonet Tilføj (+),** og klik derefter på **OK.**</span><span class="sxs-lookup"><span data-stu-id="d1ecc-108">Click the **Add (+)** icon, and then click **OK**.</span></span>
7. <span data-ttu-id="d1ecc-109">Klik på **Vælg et ud** for feltet Gør **følgende.**</span><span class="sxs-lookup"><span data-stu-id="d1ecc-109">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="d1ecc-110">Vælg **Kryptér i rullemenuen RMS-skabelon,** og klik derefter på **OK.**</span><span class="sxs-lookup"><span data-stu-id="d1ecc-110">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="d1ecc-111">(Hvis du ikke kan se denne indstilling, betyder det, at din plan ikke omfatter automatisk kryptering.</span><span class="sxs-lookup"><span data-stu-id="d1ecc-111">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="d1ecc-112">Men du kan tilføje den!)</span><span class="sxs-lookup"><span data-stu-id="d1ecc-112">But you can add it!)</span></span>
9. <span data-ttu-id="d1ecc-113">Vælg eventuelt valgfrit valg (på en liste over valgfrie valg, du kan foretage på nuværende tidspunkt, hvoraf mange kan stå med standardindstillingen for enkelhed).</span><span class="sxs-lookup"><span data-stu-id="d1ecc-113">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="d1ecc-114">Klik på **Gem**.</span><span class="sxs-lookup"><span data-stu-id="d1ecc-114">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="d1ecc-115">Du kan altid vende tilbage og redigere denne regel senere.</span><span class="sxs-lookup"><span data-stu-id="d1ecc-115">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="d1ecc-116">Du kan finde flere oplysninger om oprettelse af regler for kryptering i [Definere regler for mailflow for at kryptere mails i Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="d1ecc-116">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>