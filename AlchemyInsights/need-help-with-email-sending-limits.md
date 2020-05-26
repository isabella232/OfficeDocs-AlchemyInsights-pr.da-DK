---
title: Har du brug for hjælp til grænser for afsendelse af e-mails?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 7f563df313c869d18c3e4240d271c649a74914af
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357398"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="5c148-102">Har du brug for hjælp til grænser for afsendelse af e-mails?</span><span class="sxs-lookup"><span data-stu-id="5c148-102">Need help with email sending limits?</span></span>

<span data-ttu-id="5c148-103">Nedenfor er **by-design afsendelse grænser håndhæves** i tjenesten.</span><span class="sxs-lookup"><span data-stu-id="5c148-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="5c148-104">Du kan finde flere oplysninger om disse grænser [her](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="5c148-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="5c148-105">For at modvirke levering af uopfordrede massemeddelelser anvender vi hastighedsgrænser pr. bruger **på alle udgående og interne meddelelser**.</span><span class="sxs-lookup"><span data-stu-id="5c148-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="5c148-106">På tværs af alle lagervarer er denne grænse **10.000 modtagere om dagen.**</span><span class="sxs-lookup"><span data-stu-id="5c148-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="5c148-107">Kunder, der har brug for at sende en legitim massekommerciel e-mail (f.eks. kundenyhedsbreve), skal bruge tredjepartsudbydere, der specialiserer sig i disse tjenester.</span><span class="sxs-lookup"><span data-stu-id="5c148-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="5c148-108">**Bemærk:** Når grænsen for modtagerhastighed er nået, kan meddelelser ikke sendes fra postkassen, før antallet af modtagere, der er sendt meddelelser inden for de seneste 24 timer, falder til under grænsen.</span><span class="sxs-lookup"><span data-stu-id="5c148-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="5c148-109">Brugeren kan ikke sende meddelelser før dette tidspunkt.</span><span class="sxs-lookup"><span data-stu-id="5c148-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="5c148-110">Grænsen for meddelelseshastighed på **30 meddelelser pr. minut** anvendes på tværs af alle lagervarer.</span><span class="sxs-lookup"><span data-stu-id="5c148-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="5c148-111">Dette bestemmer, hvor mange meddelelser en bruger kan sende fra sin Exchange Online-konto inden for en bestemt periode.</span><span class="sxs-lookup"><span data-stu-id="5c148-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="5c148-112">Det maksimale antal modtagere, der er tilladt i felterne **Til, Cc og Bcc** for en enkelt mail på tværs af alle Lagervarer, er **1000 modtagere**.</span><span class="sxs-lookup"><span data-stu-id="5c148-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="5c148-113">Hvis du vil tilpasse denne grænse, skal du gå [hertil](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="5c148-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
