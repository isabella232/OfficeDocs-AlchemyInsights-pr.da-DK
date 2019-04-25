---
title: Adgangsstyring med Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 2e778bf4fbdb766700fb24b3405b4ddce89253f7
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/23/2019
ms.locfileid: "32393535"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="1dfd8-102">Adgangsstyring med Intune</span><span class="sxs-lookup"><span data-stu-id="1dfd8-102">Conditional Access with Intune</span></span>

<span data-ttu-id="1dfd8-103">Ved hjælp af **Adgangsstyring** med Intune kræver 3 trin:</span><span class="sxs-lookup"><span data-stu-id="1dfd8-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="1dfd8-104">Oprette en **Betinget af adgangspolitik** , der definerer, hvilke ressourcer beskyttes, og hvilke betingelser der skal være opfyldt for at få adgang til disse ressourcer.</span><span class="sxs-lookup"><span data-stu-id="1dfd8-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="1dfd8-105">For eksempel skal en enhed være kompatible inden adgang til virksomhedens e-mail.</span><span class="sxs-lookup"><span data-stu-id="1dfd8-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="1dfd8-106">Oprette en **Politik for overholdelse** for at definere indstillinger, der skal opfyldes, før enheden anses for at være kompatible.</span><span class="sxs-lookup"><span data-stu-id="1dfd8-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="1dfd8-107">En enhed skal have en PIN-kode på mindst 6 cifre, før den betragtes kompatible.</span><span class="sxs-lookup"><span data-stu-id="1dfd8-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="1dfd8-108">At sikre både **Overholdelse politikker** og **Betinget adgang politikker** er målrettet til de ønskede grupper af brugere.</span><span class="sxs-lookup"><span data-stu-id="1dfd8-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="1dfd8-109">Dette kan kræve oprettelse af bestemte grupper af brugere i Active Directory i Azure.</span><span class="sxs-lookup"><span data-stu-id="1dfd8-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="1dfd8-110">Læs mere:</span><span class="sxs-lookup"><span data-stu-id="1dfd8-110">Read more:</span></span>
  
- [<span data-ttu-id="1dfd8-111">Bedste fremgangsmåder for betinget adgang</span><span class="sxs-lookup"><span data-stu-id="1dfd8-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="1dfd8-112">Introduktion til betinget adgang</span><span class="sxs-lookup"><span data-stu-id="1dfd8-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

