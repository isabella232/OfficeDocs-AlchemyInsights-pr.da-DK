---
title: AntiSpam 5.4.1 DBEB catch-alle
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: 4f531a063d63aff239ef7dead869bb526e17fb35
ms.sourcegitcommit: 2591e1f56e8943bddb9d3b77ba5b494ac49d4f30
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 11/15/2019
ms.locfileid: "38672427"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="06969-102">Løs problemer med levering af fejlkode 550 5.4.1 relæ adgang nægtet</span><span class="sxs-lookup"><span data-stu-id="06969-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="06969-103">Dette problem opstår, når du [tjekker, om en e-mail-adresse er gyldig for at forhindre tilbageslag](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) , når du indtaster Office 365-netværket.</span><span class="sxs-lookup"><span data-stu-id="06969-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Office 365 network.</span></span> <span data-ttu-id="06969-104">Prøv følgende:</span><span class="sxs-lookup"><span data-stu-id="06969-104">Try the following:</span></span>

1. <span data-ttu-id="06969-105">Bestem, om problemet er specifikt for et helt domæne eller en enkelt e-mail-adresse:</span><span class="sxs-lookup"><span data-stu-id="06969-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="06969-106">Hele domænet: nogle gange skal domænet synkroniseres. Prøv at [indstille domænet til internt og derefter tilbage til autoritativ](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="06969-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="06969-107">Enkelt e-mail-adresse: nogle gange skal adressen synkroniseres. Det kan hjælpe at ændre SMTP-proxyadressen og derefter ændre den igen.</span><span class="sxs-lookup"><span data-stu-id="06969-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="06969-108">Find ud af, om problemet er specifikt for en gruppe eller en offentlig mappe.</span><span class="sxs-lookup"><span data-stu-id="06969-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="06969-109">For nogle objekttyper skal objekterne muligvis oprettes manuelt i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="06969-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="06969-110">Hvis du har brug for yderligere hjælp, skal du åbne en support billet og angive omfanget af problemet (Inkluder den type objekt, du sender til), så vi kan hjælpe dig bedre.</span><span class="sxs-lookup"><span data-stu-id="06969-110">If you need additional help, please open a support ticket and specify the scope of the issue (includidng the type of object you're sending to) so we can assist you better.</span></span>