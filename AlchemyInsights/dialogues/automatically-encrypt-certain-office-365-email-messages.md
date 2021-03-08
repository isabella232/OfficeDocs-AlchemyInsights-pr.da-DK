---
title: Kryptere visse Office 365-mails automatisk
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
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524011"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a><span data-ttu-id="0faac-102">Kryptere visse Office 365-mails automatisk</span><span class="sxs-lookup"><span data-stu-id="0faac-102">Automatically encrypt certain Office 365 email messages</span></span>

<span data-ttu-id="0faac-103">Du kan automatisk kryptere meddelelser, som brugere sender til bestemte eksterne personer eller organisationer.</span><span class="sxs-lookup"><span data-stu-id="0faac-103">You can automatically encrypt messages that users send to certain external people or organizations.</span></span> <span data-ttu-id="0faac-104">Det gør du ved at udføre følgende trin:</span><span class="sxs-lookup"><span data-stu-id="0faac-104">To do this, perform the following steps:</span></span>

1. <span data-ttu-id="0faac-105">I [Exchange Administration skal du](https://outlook.office365.com/ecp/)vælge **mailflow > regler.**</span><span class="sxs-lookup"><span data-stu-id="0faac-105">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="0faac-106">Klik på **ikonet Nyt (+),** og klik derefter på **Anvend Office 365-meddelelseskryptering og rettighedsbeskyttelse på meddelelser.**</span><span class="sxs-lookup"><span data-stu-id="0faac-106">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="0faac-107">Skriv **et navn** til reglen under Navn, f.eks. Kryptér *meddelelser, der sendes til DrToniRamos@gmail.com.*</span><span class="sxs-lookup"><span data-stu-id="0faac-107">In **Name**, enter a name for the rule, such as *Encrypt messages sent to DrToniRamos@gmail.com*.</span></span>
4. <span data-ttu-id="0faac-108">I **Anvend denne regel, hvis** skal du vælge > er denne **person.**</span><span class="sxs-lookup"><span data-stu-id="0faac-108">In **Apply this rule if**, choose **The recipient > is this person**.</span></span> 
5. <span data-ttu-id="0faac-109">Vælg navnet **på den** person, du vil anvende krypteringsreglen på, i vinduet Vælg medlemmer, og klik derefter på **Tilføj.**</span><span class="sxs-lookup"><span data-stu-id="0faac-109">In the **Select Members** window, select the name of the person you want the encryption rule to apply to, and then click **add**.</span></span> 
6. <span data-ttu-id="0faac-110">Klik på OK, når du er færdig med at tilføje **brugere.**</span><span class="sxs-lookup"><span data-stu-id="0faac-110">When you're done adding users, click **OK**.</span></span>
7. <span data-ttu-id="0faac-111">Klik på **Vælg et ud** for feltet Gør **følgende.**</span><span class="sxs-lookup"><span data-stu-id="0faac-111">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="0faac-112">Vælg **Kryptér i rullemenuen RMS-skabelon,** og klik derefter på **OK.**</span><span class="sxs-lookup"><span data-stu-id="0faac-112">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="0faac-113">(Hvis du ikke kan se denne indstilling, betyder det, at din plan ikke omfatter automatisk kryptering.</span><span class="sxs-lookup"><span data-stu-id="0faac-113">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="0faac-114">Men du kan tilføje den!)</span><span class="sxs-lookup"><span data-stu-id="0faac-114">But you can add it!)</span></span>
9. <span data-ttu-id="0faac-115">Vælg eventuelt valgfrit valg (på en liste over valgfrie valg, du kan foretage på nuværende tidspunkt, hvoraf mange kan stå med standardindstillingen for enkelhed).</span><span class="sxs-lookup"><span data-stu-id="0faac-115">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="0faac-116">Klik på **Gem**.</span><span class="sxs-lookup"><span data-stu-id="0faac-116">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="0faac-117">Du kan altid vende tilbage og redigere denne regel senere.</span><span class="sxs-lookup"><span data-stu-id="0faac-117">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="0faac-118">Du kan finde flere oplysninger om oprettelse af regler for kryptering i [Definere regler for mailflow for at kryptere mails i Office 365.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="0faac-118">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

