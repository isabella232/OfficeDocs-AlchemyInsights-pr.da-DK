---
title: Løs almindelige problemer med Microsoft Defender til Office 365
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
ms.openlocfilehash: 05fa518ece7ea40fd7b4cea57115d9cd60370b01
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744882"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a><span data-ttu-id="66efb-102">Løs almindelige problemer med Microsoft Defender til Office 365</span><span class="sxs-lookup"><span data-stu-id="66efb-102">Fix common problems with Microsoft Defender for Office 365</span></span>

<span data-ttu-id="66efb-103">Her er nogle løsninger på almindelige problemer med Microsoft Defender til Office 365:</span><span class="sxs-lookup"><span data-stu-id="66efb-103">Here are some solutions to common problems with Microsoft Defender for Office 365:</span></span>

- <span data-ttu-id="66efb-104">**Meddelelsesforsinkelse:** Hvis du oplever problemer, hvor leveringen af meddelelser forsinkes,  er det en god ide at bruge indstillingerne for dynamisk levering i politikken for sikre vedhæftede filer.</span><span class="sxs-lookup"><span data-stu-id="66efb-104">**Message delay:** If you're experiencing issues where message delivery is delayed, you'll want to use the **Dynamic Delivery** options within your Safe Attachments policy.</span></span> <span data-ttu-id="66efb-105">Du kan få mere at vide under [Dynamisk levering i politikker for sikre vedhæftede filer.](https://go.microsoft.com/fwlink/?linkid=2094106)</span><span class="sxs-lookup"><span data-stu-id="66efb-105">To learn more, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2094106).</span></span>
- <span data-ttu-id="66efb-106">**Rapportere falske positive eller negative resultater:** Rapportér meddelelsen til Microsoft ved hjælp af dette link: [Microsoft Defender Response Portal.](https://go.microsoft.com/fwlink/?linkid=2092835)</span><span class="sxs-lookup"><span data-stu-id="66efb-106">**Report false positive or negative results:** Report the message to Microsoft using this link: [Microsoft Defender Response Portal](https://go.microsoft.com/fwlink/?linkid=2092835).</span></span>
- <span data-ttu-id="66efb-107">**Aktivér beskyttelse mod sikre links:**</span><span class="sxs-lookup"><span data-stu-id="66efb-107">**Enable Safe Link protection:**</span></span>
    1. <span data-ttu-id="66efb-108">Log på [Office 365 Security & Compliance Center.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="66efb-108">Sign in to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
    2. <span data-ttu-id="66efb-109">Gå til links **til sikre politikker**  >  **for**  >  **trusselsadministration.**</span><span class="sxs-lookup"><span data-stu-id="66efb-109">Go to **Threat Management** > **Policy** > **Safe Links.**</span></span>
    3. <span data-ttu-id="66efb-110">Åbn **den konfigurerede politik under Politikker,** der gælder for bestemte modtagere.</span><span class="sxs-lookup"><span data-stu-id="66efb-110">Under **Policies that apply to specific recipients**, open the policy configured.</span></span>
    4. <span data-ttu-id="66efb-111">Under **Indstillinger skal** du vælge Anvend sikre links til **meddelelser, der sendes i organisationen.**</span><span class="sxs-lookup"><span data-stu-id="66efb-111">Under **Settings**, select **Apply safe links to messages sent within the organization**.</span></span>
