---
title: Politikken AllowSelfServicePurchase kan ikke angives eller vises
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158555"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="57677-102">Politikken AllowSelfServicePurchase kan ikke angives eller vises</span><span class="sxs-lookup"><span data-stu-id="57677-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="57677-103">Når du forsøger at angive eller få vist politikken AllowSelfServicePurchase, får du vist følgende fejlmeddelelse:</span><span class="sxs-lookup"><span data-stu-id="57677-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="57677-104">*HandleError : Produktpolitikken kunne ikke hentes med PolicyId 'AllowSelfServicePurchase', ErrorMessage - Den underliggende forbindelse blev lukket: Der opstod en uventet fejl under en afsendelse.*</span><span class="sxs-lookup"><span data-stu-id="57677-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="57677-105">Dette kan skyldes en ældre version af Transport Layer Security (TLS).</span><span class="sxs-lookup"><span data-stu-id="57677-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="57677-106">Hvis du vil tilslutte MSCommerce-tjenesten, skal du bruge TLS 1.2 eller derover.</span><span class="sxs-lookup"><span data-stu-id="57677-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="57677-107">Prøv følgende trin for at aktivere/indstille TLS-protokollen til 1.2, skal du kontrollere og prøve igen.</span><span class="sxs-lookup"><span data-stu-id="57677-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="57677-108">Ved Kommandoprompten til PowerShell\) (PS C: Angiv følgende kommando for at indstille TLS-protokollen til version 1.2:</span><span class="sxs-lookup"><span data-stu-id="57677-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="57677-109">Kontroller de TLS-protokoller, der er i brug, med følgende kommando:</span><span class="sxs-lookup"><span data-stu-id="57677-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="57677-110">Prøv kommandoerne Hent eller Opdater igen efter behov.</span><span class="sxs-lookup"><span data-stu-id="57677-110">Retry the Get or Update commands as needed.</span></span>

