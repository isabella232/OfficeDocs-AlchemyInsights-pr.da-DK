---
title: Spam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717355"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="cafde-102">Løs leverings problemer for fejlkode 550 5.4.1 Relay-adgang nægtet</span><span class="sxs-lookup"><span data-stu-id="cafde-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="cafde-103">Dette problem opstår, når du [kontrollerer, om en mailadresse er gyldig for at forhindre bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) , når du angiver Microsoft-netværket.</span><span class="sxs-lookup"><span data-stu-id="cafde-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="cafde-104">Prøv følgende:</span><span class="sxs-lookup"><span data-stu-id="cafde-104">Try the following:</span></span>

1. <span data-ttu-id="cafde-105">Find ud af, om problemet er specifikt for et helt domæne eller en enkelt mailadresse:</span><span class="sxs-lookup"><span data-stu-id="cafde-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="cafde-106">Hele domænet: nogle gange skal domænet synkroniseres. Prøv at [indstille domænet til internt og derefter tilbage til autoritativ](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="cafde-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="cafde-107">Enkelt mailadresse: det er nogle gange, at adressen skal synkroniseres. Hvis du ændrer SMTP-proxyadressen og derefter ændrer den tilbage, kan det hjælpe.</span><span class="sxs-lookup"><span data-stu-id="cafde-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="cafde-108">Find ud af, om problemet er specifikt for en gruppe eller en offentlig mappe.</span><span class="sxs-lookup"><span data-stu-id="cafde-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="cafde-109">For nogle objekttyper skal objekterne muligvis oprettes manuelt i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="cafde-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="cafde-110">Hvis du har brug for yderligere hjælp, skal du åbne en supportanmodning og angive omfanget af problemet (herunder den type objekt, du sender til), så vi kan hjælpe dig bedre.</span><span class="sxs-lookup"><span data-stu-id="cafde-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>