---
title: Ret forbindelsespolitik
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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/09/2021
ms.locfileid: "50693300"
---
# <a name="fix-connection-policy"></a><span data-ttu-id="50cda-102">Ret forbindelsespolitik</span><span class="sxs-lookup"><span data-stu-id="50cda-102">Fix connection policy</span></span>

<span data-ttu-id="50cda-103">Mailen blev markeret som sikker og leveret til brugerens indbakke, fordi den afsendende IP-adresse var markeret som sikker i politikken Forbindelsesfilter.</span><span class="sxs-lookup"><span data-stu-id="50cda-103">The email was marked safe and delivered to the user's inbox because the sending IP address was marked safe in the Connection Filter policy.</span></span> <span data-ttu-id="50cda-104">Hvis du vil gennemse politikken, skal du gøre følgende:</span><span class="sxs-lookup"><span data-stu-id="50cda-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="50cda-105">Gå til [Office 365 Security & Compliance Center,](https://go.microsoft.com/fwlink/p/?linkid=2077143)og gå derefter **til** antispam  >  **for politikker**  >  [for trusselsadministration.](https://go.microsoft.com/fwlink/?linkid=2101518)</span><span class="sxs-lookup"><span data-stu-id="50cda-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="50cda-106">Vælg **filterpolitikken** Forbindelse under fanen **Brugerdefineret, og** vælg derefter **Rediger politik.**</span><span class="sxs-lookup"><span data-stu-id="50cda-106">On the **Custom** tab, select the **Connection filter policy**, and then select **Edit policy**.</span></span>
3. <span data-ttu-id="50cda-107">Gennemse **listen over tilladte IP-adresser.**</span><span class="sxs-lookup"><span data-stu-id="50cda-107">Review the **IP Allow** list.</span></span> <span data-ttu-id="50cda-108">Se, om **listen over sikre personer** er aktiveret.</span><span class="sxs-lookup"><span data-stu-id="50cda-108">See if **Safe list** is enabled.</span></span>

    > [!NOTE]
    > <span data-ttu-id="50cda-109">Microsoft abonnerer på tredjepartskilder for afsendere, der er tillid til.</span><span class="sxs-lookup"><span data-stu-id="50cda-109">Microsoft subscribes to third-party sources of trusted senders.</span></span> <span data-ttu-id="50cda-110">Hvis **listen er** aktiveret, markeres disse afsendere, der er tillid til, ikke ved en fejltagelse som spam.</span><span class="sxs-lookup"><span data-stu-id="50cda-110">If **Safe list** is enabled, these trusted senders aren't mistakenly marked as spam.</span></span> <span data-ttu-id="50cda-111">Jeg anbefaler at vælge denne indstilling, da det vil reducere antallet af falske positive (gode mails, der er klassificeret som spam), som du modtager.</span><span class="sxs-lookup"><span data-stu-id="50cda-111">I recommend selecting this option, because it will reduce the number of false positives (good mail that's classified as spam) that you receive.</span></span>
