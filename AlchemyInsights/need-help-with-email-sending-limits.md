---
title: Har du brug for hjælp til grænser for afsendelse af mail?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: b5bdfbf818328c97ec93b3468aeedcbe88e03913
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836273"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="20a89-102">Har du brug for hjælp til grænser for afsendelse af mail?</span><span class="sxs-lookup"><span data-stu-id="20a89-102">Need help with email sending limits?</span></span>

<span data-ttu-id="20a89-103">Nedenfor er de **designbaserede grænser for afsendelse** i tjenesten.</span><span class="sxs-lookup"><span data-stu-id="20a89-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="20a89-104">Du kan finde flere oplysninger om disse begrænsninger [her.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits)</span><span class="sxs-lookup"><span data-stu-id="20a89-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="20a89-105">For at afholde os fra at levere uopfordrede massemeddelelser, anvender vi satsbegrænsninger pr. bruger **på alle udgående og interne meddelelser.**</span><span class="sxs-lookup"><span data-stu-id="20a89-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="20a89-106">På tværs af alle SKU'er er **denne grænse 10.000 modtagere pr. dag.**</span><span class="sxs-lookup"><span data-stu-id="20a89-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="20a89-107">Kunder, der har brug for at sende legitime kommercielle massemails (f.eks. kundebrevbrev), bør benytte tredjepartsudbydere, der er specialiserede i disse tjenester.</span><span class="sxs-lookup"><span data-stu-id="20a89-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="20a89-108">**Bemærk!** Når du når grænsen for modtagerhastigheden, kan meddelelser ikke sendes fra postkassen, før antallet af modtagere, der er blevet sendt meddelelser inden for de seneste 24 timer, falder under grænsen.</span><span class="sxs-lookup"><span data-stu-id="20a89-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="20a89-109">Brugeren vil ikke kunne sende meddelelser før dette tidspunkt.</span><span class="sxs-lookup"><span data-stu-id="20a89-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="20a89-110">Grænsen for **meddelelsessats på 30 meddelelser i minuttet** anvendes på tværs af alle SKU'er.</span><span class="sxs-lookup"><span data-stu-id="20a89-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="20a89-111">Dette bestemmer, hvor mange meddelelser en bruger kan sende fra sin Exchange Online-konto inden for en bestemt periode.</span><span class="sxs-lookup"><span data-stu-id="20a89-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="20a89-112">Det maksimale antal modtagere, der er tilladt i felterne **Til, Cc** og Bcc for en enkelt mail på tværs af alle SKU'er, er **1000 modtagere.**</span><span class="sxs-lookup"><span data-stu-id="20a89-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="20a89-113">Hvis du vil tilpasse denne grænse, skal du [gå hertil.](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228)</span><span class="sxs-lookup"><span data-stu-id="20a89-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
