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
ms.openlocfilehash: c9c47d71b2da3840504d5b28c7c9e067b4c05fa5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706015"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="96254-102">Betinget adgang med Intune</span><span class="sxs-lookup"><span data-stu-id="96254-102">Conditional Access with Intune</span></span>

<span data-ttu-id="96254-103">Brug **af betinget adgang** med Intune kræver tre trin:</span><span class="sxs-lookup"><span data-stu-id="96254-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="96254-104">Opret en **adgangsstyring,** der definerer, hvilke ressourcer der beskyttes, og hvilke betingelser der skal opfyldes for at få adgang til disse ressourcer.</span><span class="sxs-lookup"><span data-stu-id="96254-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="96254-105">En enhed skal f.eks.</span><span class="sxs-lookup"><span data-stu-id="96254-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="96254-106">Opret en **overholdelsespolitik** for at definere indstillinger, der skal være opfyldt, før enheden betragtes som kompatibel.</span><span class="sxs-lookup"><span data-stu-id="96254-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="96254-107">En enhed skal for eksempel have en nål på mindst 6 cifre, før den anses for at være kompatibel.</span><span class="sxs-lookup"><span data-stu-id="96254-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="96254-108">Sikring af både **overholdelsespolitikker** og **politikker for betinget adgang** er målrettet mod de ønskede grupper af brugere.</span><span class="sxs-lookup"><span data-stu-id="96254-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="96254-109">Dette kan kræve oprettelse af bestemte grupper af brugere i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="96254-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="96254-110">Læs mere:</span><span class="sxs-lookup"><span data-stu-id="96254-110">Read more:</span></span>
  
- [<span data-ttu-id="96254-111">Bedste fremgangsmåder for betinget adgang</span><span class="sxs-lookup"><span data-stu-id="96254-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="96254-112">Introduktion til Betinget adgang</span><span class="sxs-lookup"><span data-stu-id="96254-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

