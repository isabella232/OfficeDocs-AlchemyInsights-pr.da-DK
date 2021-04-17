---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821441"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="77678-102">Løs leveringsproblemer for fejlkode 550 5.4.1 Relay Access Denied</span><span class="sxs-lookup"><span data-stu-id="77678-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="77678-103">Dette problem opstår, når [du kontrollerer, om en mailadresse er](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) gyldig, for at forhindre tilbageførsel ved indtastning af Microsoft-netværket.</span><span class="sxs-lookup"><span data-stu-id="77678-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="77678-104">Prøv følgende:</span><span class="sxs-lookup"><span data-stu-id="77678-104">Try the following:</span></span>

1. <span data-ttu-id="77678-105">Afgør, om problemet er specifikt for et helt domæne eller en enkelt mailadresse:</span><span class="sxs-lookup"><span data-stu-id="77678-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="77678-106">Hele domænet: Nogle gange skal domænet synkroniseres; prøv [at indstille domænet til Intern og derefter tilbage til Autoritativ](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="77678-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="77678-107">Enkelt mailadresse: Nogle gange skal adressen synkroniseres; det kan hjælpe at ændre smtp-proxyadressen og derefter ændre den tilbage.</span><span class="sxs-lookup"><span data-stu-id="77678-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="77678-108">Afgør, om problemet er specifikt for en gruppe eller offentlig mappe.</span><span class="sxs-lookup"><span data-stu-id="77678-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="77678-109">For nogle objekttyper skal objekterne muligvis oprettes manuelt i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="77678-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="77678-110">Hvis du har brug for yderligere hjælp, skal du åbne en supportbillet og angive problemets omfang (herunder typen af objekt, du sender til), så vi kan hjælpe dig bedre.</span><span class="sxs-lookup"><span data-stu-id="77678-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>