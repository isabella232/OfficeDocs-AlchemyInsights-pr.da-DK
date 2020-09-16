---
title: Har du brug for hjælp til mail afsende begrænsninger?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 66ff82afd7b44ef5fd4943bfc794c2fa35bbfa9e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702357"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="12a2e-102">Har du brug for hjælp til mail afsende begrænsninger?</span><span class="sxs-lookup"><span data-stu-id="12a2e-102">Need help with email sending limits?</span></span>

<span data-ttu-id="12a2e-103">Herunder er de **begrænsninger, som** tildeles ved at håndhæves i tjenesten.</span><span class="sxs-lookup"><span data-stu-id="12a2e-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="12a2e-104">Yderligere oplysninger om disse begrænsninger beskrives [her](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="12a2e-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="12a2e-105">For at forhindre levering af meddelelser, der ikke blev anmodet om, gælder det, at vi anvender **tilsvarende begrænsninger pr. bruger på alle udgående og interne meddelelser**.</span><span class="sxs-lookup"><span data-stu-id="12a2e-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="12a2e-106">På tværs af alle lager numre er denne grænse **10.000 modtagere om dagen**.</span><span class="sxs-lookup"><span data-stu-id="12a2e-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="12a2e-107">Kunder, der har brug for at sende ægte kommercielle mails (f. eks. kunde-nyhedsbreve), skal anvende tredjepartsudbydere, der er specialiseret i disse tjenester.</span><span class="sxs-lookup"><span data-stu-id="12a2e-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="12a2e-108">**Bemærk**! når grænsen for modtager satsen er nået, kan meddelelser ikke sendes fra postkassen, før antallet af modtagere, der er blevet sendt meddelelser inden for de seneste 24 timer, falder ned under grænsen.</span><span class="sxs-lookup"><span data-stu-id="12a2e-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="12a2e-109">Brugeren vil ikke kunne sende meddelelser før dette tidspunkt.</span><span class="sxs-lookup"><span data-stu-id="12a2e-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="12a2e-110">Grænsen for meddelelses hastighed på **30 meddelelser pr. minut** anvendes på tværs af alle SKU'er.</span><span class="sxs-lookup"><span data-stu-id="12a2e-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="12a2e-111">Dette bestemmer, hvor mange meddelelser en bruger kan sende fra sin Exchange Online-konto inden for en bestemt periode.</span><span class="sxs-lookup"><span data-stu-id="12a2e-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="12a2e-112">Det **maksimale antal modtagere, der er tilladt i felterne til, CC og Bcc** for en enkelt mail, er **1000 modtagere**på tværs af alle SKU'er.</span><span class="sxs-lookup"><span data-stu-id="12a2e-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="12a2e-113">Du kan tilpasse denne grænse ved at gå [hertil](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="12a2e-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
