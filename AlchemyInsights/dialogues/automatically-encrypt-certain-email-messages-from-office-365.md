---
title: Kryptere bestemte mails automatisk fra Office 365
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
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524015"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a><span data-ttu-id="8b1bb-102">Kryptere bestemte mails automatisk fra Office 365</span><span class="sxs-lookup"><span data-stu-id="8b1bb-102">Automatically encrypt certain email messages from office 365</span></span>

1. <span data-ttu-id="8b1bb-103">I [Exchange Administration skal du](https://outlook.office365.com/ecp/)vælge **mailflow > regler.**</span><span class="sxs-lookup"><span data-stu-id="8b1bb-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="8b1bb-104">Klik på **ikonet Nyt (+),** og klik derefter på **Anvend Office 365-meddelelseskryptering og rettighedsbeskyttelse på meddelelser.**</span><span class="sxs-lookup"><span data-stu-id="8b1bb-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="8b1bb-105">Skriv **et** navn til reglen under Navn, f.eks. *Kryptér alle meddelelser.*</span><span class="sxs-lookup"><span data-stu-id="8b1bb-105">In **Name**, enter a name for the rule, such as *Encrypt all messages*.</span></span>
4. <span data-ttu-id="8b1bb-106">Vælg **[Anvend på alle** meddelelser] i Anvend denne **regel, hvis.**</span><span class="sxs-lookup"><span data-stu-id="8b1bb-106">In **Apply this rule if**, choose **[Apply to all messages]**.</span></span> 
5. <span data-ttu-id="8b1bb-107">Klik på **Vælg et ud** for feltet Gør **følgende.**</span><span class="sxs-lookup"><span data-stu-id="8b1bb-107">Next to the **Do the following** field, click **Select one**.</span></span> 
6. <span data-ttu-id="8b1bb-108">Vælg **Kryptér i rullemenuen RMS-skabelon,** og klik derefter på **OK.**</span><span class="sxs-lookup"><span data-stu-id="8b1bb-108">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="8b1bb-109">(Hvis du ikke kan se denne indstilling, betyder det, at din plan ikke omfatter automatisk kryptering.</span><span class="sxs-lookup"><span data-stu-id="8b1bb-109">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="8b1bb-110">Men du kan tilføje den!)</span><span class="sxs-lookup"><span data-stu-id="8b1bb-110">But you can add it!)</span></span>
7. <span data-ttu-id="8b1bb-111">Markér **afkrydsningsfeltet Overhold denne regel med alvorsniveau,** og vælg derefter det ønskede niveau.</span><span class="sxs-lookup"><span data-stu-id="8b1bb-111">Check the **Audit this rule with severity level** check box, and then select the desired level.</span></span> <span data-ttu-id="8b1bb-112">Hvis din virksomhed har kontraktmæssige forpligtelser til at sende alle mails krypteret, anbefaler jeg, at niveauet angives til **Høj.**</span><span class="sxs-lookup"><span data-stu-id="8b1bb-112">If your company has contractual obligations to send all emails encrypted, I recommend setting the level to **High**.</span></span>
8. <span data-ttu-id="8b1bb-113">Klik **på Gennemtving under Vælg en model** til denne **regel.**</span><span class="sxs-lookup"><span data-stu-id="8b1bb-113">Under **Choose a model for this rule**, click **Enforce**.</span></span> 
9. <span data-ttu-id="8b1bb-114">Vælg eventuelt valgfrit valg (på en liste over valgfrie valg, du kan foretage på nuværende tidspunkt, hvoraf mange kan stå med standardindstillingen for enkelhed).</span><span class="sxs-lookup"><span data-stu-id="8b1bb-114">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="8b1bb-115">Klik på **Gem**.</span><span class="sxs-lookup"><span data-stu-id="8b1bb-115">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="8b1bb-116">Du kan altid vende tilbage og redigere denne regel senere.</span><span class="sxs-lookup"><span data-stu-id="8b1bb-116">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="8b1bb-117">Du kan finde flere oplysninger om oprettelse af regler for kryptering i [Definere regler for mailflow for at kryptere mails i Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="8b1bb-117">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>

