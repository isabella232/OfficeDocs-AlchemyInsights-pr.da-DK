---
title: Det er ikke muligt at angive eller få vist AllowSelfServicePurchase-politikken
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
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735193"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="aefac-102">Det er ikke muligt at angive eller få vist AllowSelfServicePurchase-politikken</span><span class="sxs-lookup"><span data-stu-id="aefac-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="aefac-103">Når du forsøger at angive eller få vist AllowSelfServicePurchase-politikken, får du vist følgende fejlmeddelelse:</span><span class="sxs-lookup"><span data-stu-id="aefac-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="aefac-104">*HandleError: det lykkedes ikke at hente produktpolitik med PolicyId ' AllowSelfServicePurchase ', ErrorMessage-den underliggende forbindelse blev lukket: der opstod en uventet fejl i en Send.*</span><span class="sxs-lookup"><span data-stu-id="aefac-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="aefac-105">Dette kan skyldes en ældre version af TLS (Transport Layer Security).</span><span class="sxs-lookup"><span data-stu-id="aefac-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="aefac-106">Hvis du vil oprette forbindelse til MSCommerce-tjenesten, skal du bruge TLS 1,2 eller nyere.</span><span class="sxs-lookup"><span data-stu-id="aefac-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="aefac-107">Benyt følgende fremgangsmåde for at aktivere/konfigurere TLS-protokollen til 1,2, bekræfte og prøve igen.</span><span class="sxs-lookup"><span data-stu-id="aefac-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="aefac-108">Ved kommandoprompten i PowerShell (PS C: \) Skriv følgende kommando for at indstille TLS-protokollen til version 1,2:</span><span class="sxs-lookup"><span data-stu-id="aefac-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="aefac-109">Bekræft de TLS-protokoller, der er i brug, med følgende kommando:</span><span class="sxs-lookup"><span data-stu-id="aefac-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="aefac-110">Prøv kommandoerne Hent eller Opdater efter behov.</span><span class="sxs-lookup"><span data-stu-id="aefac-110">Retry the Get or Update commands as needed.</span></span>

