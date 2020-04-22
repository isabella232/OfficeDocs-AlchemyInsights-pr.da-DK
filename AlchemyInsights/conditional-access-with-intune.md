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
# <a name="conditional-access-with-intune"></a>Betinget adgang med Intune

Brug **af betinget adgang** med Intune kræver tre trin: 
  
- Opret en **adgangsstyring,** der definerer, hvilke ressourcer der beskyttes, og hvilke betingelser der skal opfyldes for at få adgang til disse ressourcer. En enhed skal f.eks. 
    
- Opret en **overholdelsespolitik** for at definere indstillinger, der skal være opfyldt, før enheden betragtes som kompatibel. En enhed skal for eksempel have en nål på mindst 6 cifre, før den anses for at være kompatibel. 
    
- Sikring af både **overholdelsespolitikker** og **politikker for betinget adgang** er målrettet mod de ønskede grupper af brugere. Dette kan kræve oprettelse af bestemte grupper af brugere i Azure Active Directory. 
    
Læs mere:
  
- [Bedste fremgangsmåder for betinget adgang](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Introduktion til Betinget adgang](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

