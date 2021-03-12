---
title: Betinget adgang med Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 20ef8205431aad821419f2559be3402c8228d838
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704780"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="f2f58-102">Betinget adgang med Intune</span><span class="sxs-lookup"><span data-stu-id="f2f58-102">Conditional Access with Intune</span></span>

<span data-ttu-id="f2f58-103">Brug  **af Betinget adgang**  med Intune kræver tre trin:</span><span class="sxs-lookup"><span data-stu-id="f2f58-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="f2f58-104">Opret en  **politik for overholdelse**  af regler og standarder [(Android,](https://docs.microsoft.com/intune/compliance-policy-create-android)  [iOS,](https://docs.microsoft.com/intune/compliance-policy-create-ios)  [Windows)](https://docs.microsoft.com//intune/compliance-policy-create-windows)for at definere indstillinger, der skal opfyldes, før enheden betragtes som værende kompatibel.</span><span class="sxs-lookup"><span data-stu-id="f2f58-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="f2f58-105">En enhed skal f.eks. have en pinkode på mindst 6 cifre, før den betragtes som værende kompatibel.</span><span class="sxs-lookup"><span data-stu-id="f2f58-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="f2f58-106">Opret en **politik for betinget adgang,**  der definerer, hvilke ressourcer der beskyttes, og hvilke betingelser der skal være opfyldt for at få adgang til disse ressourcer.</span><span class="sxs-lookup"><span data-stu-id="f2f58-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="f2f58-107">[Eksempelvis skal en enhed](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  være kompatibel, før den får adgang til virksomhedens mail.</span><span class="sxs-lookup"><span data-stu-id="f2f58-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="f2f58-108">Sørg **for, at både overholdelsespolitikker**  **og betingede**  adgangspolitikker er rettet mod de ønskede grupper af brugere.</span><span class="sxs-lookup"><span data-stu-id="f2f58-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="f2f58-109">Dette kræver muligvis oprettelse af bestemte grupper af brugere i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f2f58-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="f2f58-110">**Nyttige links:**</span><span class="sxs-lookup"><span data-stu-id="f2f58-110">**Helpful links:**</span></span>

[<span data-ttu-id="f2f58-111">Oversigt over enhedsoverholdelse</span><span class="sxs-lookup"><span data-stu-id="f2f58-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="f2f58-112">Fejlfindings-nøglecenter</span><span class="sxs-lookup"><span data-stu-id="f2f58-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="f2f58-113">Fejlfindingspolitik</span><span class="sxs-lookup"><span data-stu-id="f2f58-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="f2f58-114">For at beskytte mail (Exchange Online) mod adgang fra enheder, der ikke er lige så relevante, skal begge dokumenter følges:</span><span class="sxs-lookup"><span data-stu-id="f2f58-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="f2f58-115">Beskyt mailadgang fra enheder, der bruger EAS</span><span class="sxs-lookup"><span data-stu-id="f2f58-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="f2f58-116">Beskyt mailadgang fra enheder, der bruger moderne godkendelsesklienter som Outlook</span><span class="sxs-lookup"><span data-stu-id="f2f58-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)