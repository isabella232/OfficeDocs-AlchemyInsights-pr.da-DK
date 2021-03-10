---
title: Brug af Betinget adgang med Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692974"
---
# <a name="using-conditional-access-with-intune"></a><span data-ttu-id="03d85-102">Brug af Betinget adgang med Intune</span><span class="sxs-lookup"><span data-stu-id="03d85-102">Using Conditional Access with Intune</span></span>

<span data-ttu-id="03d85-103">Brug af Betinget adgang med Intune kræver tre trin:</span><span class="sxs-lookup"><span data-stu-id="03d85-103">Using Conditional Access with Intune requires 3 steps:</span></span>

- [<span data-ttu-id="03d85-104">Opret en politik for overholdelse af regler og standarder for at definere de indstillinger, der skal være opfyldt, før enheden betragtes som værende kompatibel. En enhed skal f.eks. have en pinkode på mindst 6 cifre, før den betragtes som værende kompatibel.</span><span class="sxs-lookup"><span data-stu-id="03d85-104">Create a Compliance Policy to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [<span data-ttu-id="03d85-105">Opret en politik for betinget adgang, der definerer, hvilke ressourcer der beskyttes, og hvilke betingelser der skal være opfyldt for at få adgang til disse ressourcer. Eksempelvis skal en enhed være kompatibel, før den får adgang til virksomhedens mail.</span><span class="sxs-lookup"><span data-stu-id="03d85-105">Create a Conditional Access Policy that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span>](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [<span data-ttu-id="03d85-106">Sørg for, at både overholdelsespolitikker og betingede adgangspolitikker er rettet mod de ønskede grupper af brugere. Dette kræver muligvis oprettelse af bestemte grupper af brugere i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="03d85-106">Ensure both Compliance Policies and Conditional Access Policies are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[<span data-ttu-id="03d85-107">Læs mere...</span><span class="sxs-lookup"><span data-stu-id="03d85-107">Read more...</span></span>](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
