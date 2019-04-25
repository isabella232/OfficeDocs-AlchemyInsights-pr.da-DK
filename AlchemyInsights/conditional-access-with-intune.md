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
# <a name="conditional-access-with-intune"></a>Adgangsstyring med Intune

Ved hjælp af **Adgangsstyring** med Intune kræver 3 trin: 
  
- Oprette en **Betinget af adgangspolitik** , der definerer, hvilke ressourcer beskyttes, og hvilke betingelser der skal være opfyldt for at få adgang til disse ressourcer. For eksempel skal en enhed være kompatible inden adgang til virksomhedens e-mail. 
    
- Oprette en **Politik for overholdelse** for at definere indstillinger, der skal opfyldes, før enheden anses for at være kompatible. En enhed skal have en PIN-kode på mindst 6 cifre, før den betragtes kompatible. 
    
- At sikre både **Overholdelse politikker** og **Betinget adgang politikker** er målrettet til de ønskede grupper af brugere. Dette kan kræve oprettelse af bestemte grupper af brugere i Active Directory i Azure. 
    
Læs mere:
  
- [Bedste fremgangsmåder for betinget adgang](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Introduktion til betinget adgang](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

