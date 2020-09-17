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
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807653"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="61f61-102">Betinget adgang med Intune</span><span class="sxs-lookup"><span data-stu-id="61f61-102">Conditional Access with Intune</span></span>

<span data-ttu-id="61f61-103">Brug af  **betinget adgang**  med Intune kræver 3 trin:</span><span class="sxs-lookup"><span data-stu-id="61f61-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="61f61-104">Opret en  **overholdelses politik**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) for at definere indstillinger, der skal opfyldes, før enheden anses for at være kompatibel.</span><span class="sxs-lookup"><span data-stu-id="61f61-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="61f61-105">For eksempel skal en enhed have en pinkode på mindst 6 cifre, før den anses for at være kompatibel.</span><span class="sxs-lookup"><span data-stu-id="61f61-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="61f61-106">Opret en **politik for betinget adgang**  , der definerer, hvilke ressourcer der beskyttes, og hvilke betingelser der skal opfyldes for at få adgang til disse ressourcer.</span><span class="sxs-lookup"><span data-stu-id="61f61-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="61f61-107">[For eksempel](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  skal en enhed være kompatibel, før du kan få adgang til virksomhedens mail.</span><span class="sxs-lookup"><span data-stu-id="61f61-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="61f61-108">Sørg for, at både **overholdelsespolitikker**  og  **politikker for betinget adgang**  er målrettet til de ønskede grupper af brugere.</span><span class="sxs-lookup"><span data-stu-id="61f61-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="61f61-109">Dette kan kræve, at du opretter bestemte grupper af brugere i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="61f61-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="61f61-110">**Nyttige links:**</span><span class="sxs-lookup"><span data-stu-id="61f61-110">**Helpful links:**</span></span>

[<span data-ttu-id="61f61-111">Oversigt over enheds overholdelse</span><span class="sxs-lookup"><span data-stu-id="61f61-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="61f61-112">Fejlfindings NØGLECENTER</span><span class="sxs-lookup"><span data-stu-id="61f61-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="61f61-113">Fejlfindings politik</span><span class="sxs-lookup"><span data-stu-id="61f61-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="61f61-114">Hvis du vil beskytte mail (Exchange Online) fra Access fra ikke-kompatible enheder, skal begge dokumenter følges:</span><span class="sxs-lookup"><span data-stu-id="61f61-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="61f61-115">Beskytte mail adgang fra enheder ved hjælp af EA</span><span class="sxs-lookup"><span data-stu-id="61f61-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="61f61-116">Beskytte mail adgang fra enheder, der bruger moderne godkendelses klienter som Outlook</span><span class="sxs-lookup"><span data-stu-id="61f61-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)