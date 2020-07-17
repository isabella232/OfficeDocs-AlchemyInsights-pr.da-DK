---
title: Betinget adgang med Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931424"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="52b55-102">Betinget adgang med Intune</span><span class="sxs-lookup"><span data-stu-id="52b55-102">Conditional Access with Intune</span></span>

<span data-ttu-id="52b55-103">Brug af **betinget adgang** med Intune kræver 3 trin:</span><span class="sxs-lookup"><span data-stu-id="52b55-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="52b55-104">Opret en **overholdelsespolitik** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) for at definere indstillinger, der skal være opfyldt, før enheden anses for at være kompatibel.</span><span class="sxs-lookup"><span data-stu-id="52b55-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="52b55-105">For eksempel skal en enhed have en nål på mindst 6 cifre, før den anses for at være kompatibel.</span><span class="sxs-lookup"><span data-stu-id="52b55-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="52b55-106">Opret en **politik for betinget adgang,** der definerer, hvilke ressourcer der beskyttes, og hvilke betingelser der skal opfyldes for at få adgang til disse ressourcer.</span><span class="sxs-lookup"><span data-stu-id="52b55-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="52b55-107">For eksempel skal en enhed være [kompatibel,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) før du får adgang til virksomhedens e-mail.</span><span class="sxs-lookup"><span data-stu-id="52b55-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="52b55-108">Sørg **for,** at både overholdelsespolitikker og **politikker for betinget adgang** målrettes mod de ønskede brugergrupper.</span><span class="sxs-lookup"><span data-stu-id="52b55-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="52b55-109">Dette kan kræve, at der oprettes bestemte grupper af brugere i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="52b55-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="52b55-110">**Nyttige links:**</span><span class="sxs-lookup"><span data-stu-id="52b55-110">**Helpful links:**</span></span>

[<span data-ttu-id="52b55-111">Oversigt over overholdelse af enhed</span><span class="sxs-lookup"><span data-stu-id="52b55-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="52b55-112">Fejlfinding i forbindelse med nøglecenter</span><span class="sxs-lookup"><span data-stu-id="52b55-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="52b55-113">Fejlfindingspolitik</span><span class="sxs-lookup"><span data-stu-id="52b55-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="52b55-114">For at beskytte e-mail (Exchange online) mod adgang for ikke-koverensstemmelsesenheder skal begge dokumenter følges:</span><span class="sxs-lookup"><span data-stu-id="52b55-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="52b55-115">Beskyt e-mailadgang mod enheder, der bruger EAS</span><span class="sxs-lookup"><span data-stu-id="52b55-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="52b55-116">Beskyt mailadgang fra enheder ved hjælp af moderne godkendelsesklienter som Outlook</span><span class="sxs-lookup"><span data-stu-id="52b55-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)