---
title: Udgående relaypulje
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/08/2021
ms.locfileid: "53381631"
---
# <a name="outbound-relay-pool"></a><span data-ttu-id="0eb59-102">Udgående relaypulje</span><span class="sxs-lookup"><span data-stu-id="0eb59-102">Outbound relay pool</span></span>

<span data-ttu-id="0eb59-103">Microsoft foretager nogle ændringer i konfigurationen til videresendelse eller videresendelse af mail via Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0eb59-103">Microsoft is making some changes to the configuration for relaying or forwarding email through Microsoft 365.</span></span> <span data-ttu-id="0eb59-104">Meddelelser i visse scenarier videresendes eller videresendes via Microsoft 365 ved hjælp af en særlig relæpulje.</span><span class="sxs-lookup"><span data-stu-id="0eb59-104">Messages in certain scenarios are forwarded or relayed through Microsoft 365 using a special relay pool.</span></span> <span data-ttu-id="0eb59-105">Meddelelser, der sendes ved hjælp af relaygruppen, kan ende i modtagerens mappe med uønsket mail.</span><span class="sxs-lookup"><span data-stu-id="0eb59-105">Messages sent by using the relay pool could end up in recipient's junk mail folder.</span></span> <span data-ttu-id="0eb59-106">Få mere at vide under [Udgående leveringspuljer](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span><span class="sxs-lookup"><span data-stu-id="0eb59-106">For more information, see [Outbound delivery pools](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span></span>

<span data-ttu-id="0eb59-107">For at undgå et scenarie med brug af relæpuljen skal du kontrollere, at videresendte/videresendte meddelelser opfylder et af følgende kriterier:</span><span class="sxs-lookup"><span data-stu-id="0eb59-107">To avoid a scenario using the relay pool, make sure that forwarded/relayed messages meet one of the following criteria:</span></span>

- <span data-ttu-id="0eb59-108">Den udgående afsender er et accepteret domæne for lejeren.</span><span class="sxs-lookup"><span data-stu-id="0eb59-108">The outbound sender is an accepted domain of the tenant.</span></span>
- <span data-ttu-id="0eb59-109">SPF (Sender Policy Framework) overføres, når meddelelsen kommer til at Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0eb59-109">Sender Policy Framework (SPF) passes when the message comes to Microsoft 365.</span></span>
- <span data-ttu-id="0eb59-110">DomainKeys Identified Mail (DKIM) på P2-afsenderdomænet passerer, når meddelelsen kommer Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0eb59-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span></span>
 
<span data-ttu-id="0eb59-111">Meddelelser, der opfylder ovenstående kriterier, videresendes ikke gennem relæpuljen.</span><span class="sxs-lookup"><span data-stu-id="0eb59-111">Messages that meet the above criteria are not relayed through the relay pool.</span></span>

<span data-ttu-id="0eb59-112">Hvis MX-posten for dit domæne peges på en tredjepartsserver eller en lokal server, skal du bruge udvidet filtrering for at sikre, at SPF-valideringen er korrekt for indgående mails, og for at undgå at sende mails via relæpuljen.</span><span class="sxs-lookup"><span data-stu-id="0eb59-112">If the MX record for your domain is pointed to a third-party or on-premises server, use enhanced filtering to make sure the SPF validation is correct for inbound email and to avoid sending email through the relay pool.</span></span>

<span data-ttu-id="0eb59-113">**Hvordan kan vi se, om vi er påvirket af relæpuljen?**</span><span class="sxs-lookup"><span data-stu-id="0eb59-113">**How can we tell if we're impacted by the relay pool?**</span></span>

<span data-ttu-id="0eb59-114">Hvis dine videresendte eller videresendte mails bruger et af ovenstående kriterier, videresendes meddelelser ikke gennem relæpuljen.</span><span class="sxs-lookup"><span data-stu-id="0eb59-114">If your forwarded or relayed emails use one of the above criteria, messages won't be relayed through the relay pool.</span></span> <span data-ttu-id="0eb59-115">Men hvis en meddelelse sendes gennem en relæpulje, er udgående server-IP i området 40.95.0.0/16, og navnet på den udgående server inkluderer **rly** i navnet.</span><span class="sxs-lookup"><span data-stu-id="0eb59-115">However, if a message is sent through a relay pool, the outbound server IP is in the 40.95.0.0/16 range and the outbound server name includes **rly** in the name.</span></span>

