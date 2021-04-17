---
title: Kan ikke indstille eller få vist politikken AllowSelfServicePurchase
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
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826085"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="e528f-102">Kan ikke indstille eller få vist politikken AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="e528f-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="e528f-103">Når du forsøger at indstille eller få vist politikken AllowSelfServicePurchase, modtager du følgende fejlmeddelelse:</span><span class="sxs-lookup"><span data-stu-id="e528f-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="e528f-104">*Håndteringsfejl: Produktpolitikken kunne ikke hentes med PolicyId 'AllowSelfServicePurchase', ErrorMessage – Den underliggende forbindelse blev lukket: Der opstod en uventet fejl ved en afsendelse.*</span><span class="sxs-lookup"><span data-stu-id="e528f-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="e528f-105">Dette kan skyldes en ældre version af TLS (Transport Layer Security).</span><span class="sxs-lookup"><span data-stu-id="e528f-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="e528f-106">Hvis du vil oprette forbindelse til MSCommerce-tjenesten, skal du bruge TLS 1.2 eller derover.</span><span class="sxs-lookup"><span data-stu-id="e528f-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="e528f-107">Prøv følgende trin for at aktivere/indstille TLS-protokollen til 1.2, bekræfte og prøve igen.</span><span class="sxs-lookup"><span data-stu-id="e528f-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="e528f-108">Ved PowerShell-kommandoprompten (PS C: skal du angive følgende kommando for at indstille \) TLS-protokollen til version 1.2:</span><span class="sxs-lookup"><span data-stu-id="e528f-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="e528f-109">Bekræft, at TLS-protokollen/-protokollen(er) er i brug, med følgende kommando:</span><span class="sxs-lookup"><span data-stu-id="e528f-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="e528f-110">Prøv igen kommandoerne Hent eller Opdater efter behov.</span><span class="sxs-lookup"><span data-stu-id="e528f-110">Retry the Get or Update commands as needed.</span></span>

