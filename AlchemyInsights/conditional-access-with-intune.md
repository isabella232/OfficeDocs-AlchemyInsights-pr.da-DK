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
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36504988"
---
# <a name="conditional-access-with-intune"></a>Adgangsstyring med Intune

Ved hjælp af **Adgangsstyring** med Intune kræver 3 trin: 
  
- Oprette en **Betinget af adgangspolitik** , der definerer, hvilke ressourcer beskyttes, og hvilke betingelser der skal være opfyldt for at få adgang til disse ressourcer. For eksempel skal en enhed være kompatible inden adgang til virksomhedens e-mail. 
    
- Oprette en **Politik for overholdelse** for at definere indstillinger, der skal opfyldes, før enheden anses for at være kompatible. En enhed skal have en PIN-kode på mindst 6 cifre, før den betragtes kompatible. 
    
- At sikre både **Overholdelse politikker** og **Betinget adgang politikker** er målrettet til de ønskede grupper af brugere. Dette kan kræve oprettelse af bestemte grupper af brugere i Active Directory i Azure. 
    
Læs mere:
  
- [Bedste fremgangsmåder for betinget adgang](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Introduktion til betinget adgang](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

