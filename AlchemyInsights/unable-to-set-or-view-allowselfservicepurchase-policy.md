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
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091682"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="77e96-102">Politikken AllowSelfServicePurchase kan ikke angives eller vises</span><span class="sxs-lookup"><span data-stu-id="77e96-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="77e96-103">Når du forsøger at angive eller få vist politikken AllowSelfServicePurchase, får du vist følgende fejlmeddelelse:</span><span class="sxs-lookup"><span data-stu-id="77e96-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="77e96-104">*HandleError : Produktpolitikken kunne ikke hentes med PolicyId 'AllowSelfServicePurchase', ErrorMessage - Den underliggende forbindelse blev lukket: Der opstod en uventet fejl under en afsendelse.*</span><span class="sxs-lookup"><span data-stu-id="77e96-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="77e96-105">Dette kan skyldes en ældre version af Transport Layer Security (TLS).</span><span class="sxs-lookup"><span data-stu-id="77e96-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="77e96-106">Hvis du vil tilslutte MSCommerce-tjenesten, skal du bruge TLS 1.2 eller derover.</span><span class="sxs-lookup"><span data-stu-id="77e96-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="77e96-107">Prøv følgende trin for at aktivere/indstille TLS-protokollen til 1.2, skal du kontrollere og prøve igen.</span><span class="sxs-lookup"><span data-stu-id="77e96-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="77e96-108">Ved Kommandoprompten til PowerShell\) (PS C: Angiv følgende kommando for at indstille TLS-protokollen til version 1.2:</span><span class="sxs-lookup"><span data-stu-id="77e96-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    <span data-ttu-id="77e96-109">\[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12</span><span class="sxs-lookup"><span data-stu-id="77e96-109">\[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12</span></span>

2. <span data-ttu-id="77e96-110">Kontroller de TLS-protokoller, der er i brug, med følgende kommando:</span><span class="sxs-lookup"><span data-stu-id="77e96-110">Verify the TLS protocol(s) in use, with the following command:</span></span>

    <span data-ttu-id="77e96-111">\[Net.ServicePointManager]::SecurityProtocol</span><span class="sxs-lookup"><span data-stu-id="77e96-111">\[Net.ServicePointManager]::SecurityProtocol</span></span> 

3. <span data-ttu-id="77e96-112">Prøv kommandoerne Hent eller Opdater igen efter behov.</span><span class="sxs-lookup"><span data-stu-id="77e96-112">Retry the Get or Update commands as needed.</span></span>

