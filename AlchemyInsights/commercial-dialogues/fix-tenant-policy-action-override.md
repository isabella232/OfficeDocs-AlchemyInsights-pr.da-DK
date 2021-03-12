---
title: Ret lejerpolitik (tilsidesættelse af handling)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744479"
---
# <a name="fix-tenant-policy-action-override"></a><span data-ttu-id="99bbf-102">Ret lejerpolitik (tilsidesættelse af handling)</span><span class="sxs-lookup"><span data-stu-id="99bbf-102">Fix Tenant policy (action override)</span></span>

<span data-ttu-id="99bbf-103">En antispampolitik i din lejer har påvirket denne meddelelse.</span><span class="sxs-lookup"><span data-stu-id="99bbf-103">An anti-spam policy in your tenant affected this message.</span></span> <span data-ttu-id="99bbf-104">Hvis du vil gennemse politikken, skal du gøre følgende:</span><span class="sxs-lookup"><span data-stu-id="99bbf-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="99bbf-105">Gå til [Office 365 Security & Compliance Center,](https://go.microsoft.com/fwlink/p/?linkid=2077143)og gå derefter til antispam **for**  >    >  [politikker for trusselsadministration.](https://go.microsoft.com/fwlink/?linkid=2101518)</span><span class="sxs-lookup"><span data-stu-id="99bbf-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="99bbf-106">Kontrollér, om  politikkilden angiver følgende: Meddelelsen **Add-Xheader/ModifySubject/Redirect/Delete/No action/BCC**</span><span class="sxs-lookup"><span data-stu-id="99bbf-106">Check to see if **Policy source** indicates the following:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span></span>

    <span data-ttu-id="99bbf-107">Hvis det er ja, skal **du under** fanen Brugerdefineret kontrollere indstillingerne for den politik, der har påvirket meddelelsen.</span><span class="sxs-lookup"><span data-stu-id="99bbf-107">If so, on the **Custom** tab, check the settings of the policy that affected the message.</span></span> <span data-ttu-id="99bbf-108">Det er muligt, at standardindstillingerne **for alle** Exchange Online Protection-kunder påvirkede meddelelsen.</span><span class="sxs-lookup"><span data-stu-id="99bbf-108">It's possible that the **Standard settings** applied to all Exchange Online Protection customers affected the message.</span></span>

<span data-ttu-id="99bbf-109">Du kan finde flere oplysninger om konfiguration af politikker for spamfilter i [Konfigurere politikker for spamfiltrering.](https://go.microsoft.com/fwlink/?linkid=2101431)</span><span class="sxs-lookup"><span data-stu-id="99bbf-109">For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span></span>
