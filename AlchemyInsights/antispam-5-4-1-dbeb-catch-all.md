---
title: AntiSpam 5.4.1 DBEB catch-all
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
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707905"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="28f2f-102">Løs leveringsproblemer for fejlkode 550 5.4.1 Relay Access Denied</span><span class="sxs-lookup"><span data-stu-id="28f2f-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="28f2f-103">Dette problem opstÃ¥r, [nÃ¥r du kontrollerer, om en mailadresse er gyldig for at forhindre afvisninger,](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) nÃ¥r du kommer ind i Microsoft-netværket.</span><span class="sxs-lookup"><span data-stu-id="28f2f-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="28f2f-104">Prøv følgende:</span><span class="sxs-lookup"><span data-stu-id="28f2f-104">Try the following:</span></span>

1. <span data-ttu-id="28f2f-105">Find ud af, om problemet er specifikt for et helt domæne eller en enkelt mailadresse:</span><span class="sxs-lookup"><span data-stu-id="28f2f-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="28f2f-106">Hele domænet: Nogle gange skal domænet synkroniseres. prøv [at indstille domænet til Intern og derefter tilbage til Autoritativ](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="28f2f-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="28f2f-107">Enkelt e-mail-adresse: Nogle gange skal adressen synkroniseres. ændre smtp proxy-adresse og derefter ændre det tilbage kan hjælpe.</span><span class="sxs-lookup"><span data-stu-id="28f2f-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="28f2f-108">Find ud af, om problemet er specifikt for en gruppe eller en offentlig mappe.</span><span class="sxs-lookup"><span data-stu-id="28f2f-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="28f2f-109">For nogle objekttyper skal objekterne muligvis oprettes manuelt i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="28f2f-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="28f2f-110">Hvis du har brug for yderligere hjælp, skal du åbne en supportbillet og angive problemets omfang (herunder den type objekt, du sender til), så vi kan hjælpe dig bedre.</span><span class="sxs-lookup"><span data-stu-id="28f2f-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>