---
title: Brug af DLP i transportregler
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
- "9002635"
- "5153"
ms.openlocfilehash: e512b36b34c5fc4931fb0f796790ee4b01c6443c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827210"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="7ef36-102">Brug af DLP i transportregler</span><span class="sxs-lookup"><span data-stu-id="7ef36-102">Using DLP in transport rules</span></span>

<span data-ttu-id="7ef36-103">Hvis du vil integrere forebyggelse af datatab (DLP) til en eksisterende transport, skal du bruge betingelsen "**Hvis meddelelsen indeholder...følsomme oplysninger**" i indstillingen Transportregel.</span><span class="sxs-lookup"><span data-stu-id="7ef36-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="7ef36-104">**Du kan finde flere oplysninger i:**</span><span class="sxs-lookup"><span data-stu-id="7ef36-104">**For more details, see:**</span></span>

- <span data-ttu-id="7ef36-105">Integrerede DLP-følsomme oplysningstyper i transportregler: [Integrer regler om følsomme oplysninger](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="7ef36-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="7ef36-106">Du kan også teste reglen med eller uden politiktest ved hjælp af testtilstand på reglen.</span><span class="sxs-lookup"><span data-stu-id="7ef36-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="7ef36-107">Du skal vente 30 minutter, efter at du har oprettet reglen, før du tester den.</span><span class="sxs-lookup"><span data-stu-id="7ef36-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="7ef36-108">Se [Test regler for mailflow/transport](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="7ef36-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="7ef36-109">**Bemærk**: Hvis du forsøger at implementere en ny DLP-politik med transportregler i EAC, kan du bruge [DLP-politikker i sikkerheds- og overholdelsescenter](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) i stedet.</span><span class="sxs-lookup"><span data-stu-id="7ef36-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
