---
title: Betinget adgang med Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 11/15/2019
ms.locfileid: "36504988"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="2f19d-102">Betinget adgang med Intune</span><span class="sxs-lookup"><span data-stu-id="2f19d-102">Conditional Access with Intune</span></span>

<span data-ttu-id="2f19d-103">Brug af **betinget adgang** med Intune kræver 3 trin:</span><span class="sxs-lookup"><span data-stu-id="2f19d-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="2f19d-104">Opret en **politik for betinget adgang** , der definerer, hvilke ressourcer der beskyttes, og hvilke betingelser der skal opfyldes for at få adgang til disse ressourcer.</span><span class="sxs-lookup"><span data-stu-id="2f19d-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="2f19d-105">For eksempel skal en enhed være kompatibel, før den kan få adgang til virksomhedens e-mail.</span><span class="sxs-lookup"><span data-stu-id="2f19d-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="2f19d-106">Opret en **overholdelses politik** for at definere indstillinger, der skal være opfyldt, før enheden anses for at være kompatibel.</span><span class="sxs-lookup"><span data-stu-id="2f19d-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="2f19d-107">En enhed skal for eksempel have en pinkode på mindst 6 cifre, før den anses for at være kompatibel.</span><span class="sxs-lookup"><span data-stu-id="2f19d-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="2f19d-108">At sikre, at både **overholdelses politikker** og **politikker** for adgangsstyring målrettes mod de ønskede brugergrupper.</span><span class="sxs-lookup"><span data-stu-id="2f19d-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="2f19d-109">Dette kan kræve, at du opretter bestemte grupper af brugere i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2f19d-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="2f19d-110">Læs mere:</span><span class="sxs-lookup"><span data-stu-id="2f19d-110">Read more:</span></span>
  
- [<span data-ttu-id="2f19d-111">Bedste fremgangsmåder for betinget adgang</span><span class="sxs-lookup"><span data-stu-id="2f19d-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="2f19d-112">Introduktion til betinget adgang</span><span class="sxs-lookup"><span data-stu-id="2f19d-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

