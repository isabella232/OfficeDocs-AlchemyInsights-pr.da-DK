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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/18/2019
ms.locfileid: "36504988"
---
# <a name="conditional-access-with-intune"></a>Betinget adgang med Intune

Brug af **betinget adgang** med Intune kræver 3 trin: 
  
- Opret en **politik for betinget adgang** , der definerer, hvilke ressourcer der beskyttes, og hvilke betingelser der skal opfyldes for at få adgang til disse ressourcer. For eksempel skal en enhed være kompatibel, før den kan få adgang til virksomhedens e-mail. 
    
- Opret en **overholdelses politik** for at definere indstillinger, der skal være opfyldt, før enheden anses for at være kompatibel. En enhed skal for eksempel have en pinkode på mindst 6 cifre, før den anses for at være kompatibel. 
    
- At sikre, at både **overholdelses politikker** og **politikker** for adgangsstyring målrettes mod de ønskede brugergrupper. Dette kan kræve, at du opretter bestemte grupper af brugere i Azure Active Directory. 
    
Læs mere:
  
- [Bedste fremgangsmåder for betinget adgang](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Introduktion til betinget adgang](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

