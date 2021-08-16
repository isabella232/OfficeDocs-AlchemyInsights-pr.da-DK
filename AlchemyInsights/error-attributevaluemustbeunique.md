---
title: FejlattributVærdiMustBeUnique
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 37d6764d19d9cfbb0899a5ab85a4b1530896568adc364122075b7d6f2a32970a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54002114"
---
# <a name="error-attributevaluemustbeunique"></a>Fejl: AttributVærdiMustBeUnique

Den mest almindelige årsag til fejlen AttributVærdiMustBeUnique er to objekter med forskellige SourceAnchor (immutableId) har den samme værdi for attributterne ProxyAddresses og/eller UserPrincipalName. Sådan retter du fejlen AttributVærdiMustBeUnique:
  
1. Identificer de duplikerede proxyAddresses, userPrincipalName eller en anden attributværdi, der forårsager fejlen. Identificer også, hvilke to (eller flere) objekter, der er involveret i konflikten. Den rapport, der genereres af Azure AD Forbind Health for sync, kan hjælpe dig med at identificere de to objekter.
    
2. Identificer, hvilket objekt der fortsat skal have den duplikerede værdi, og hvilket objekt der ikke skal have.
    
3. Fjern den duplikerede værdi fra det objekt, der IKKE skal have den pågældende værdi. Bemærk, at du skal foretage ændringen i den mappe, hvor objektet kommer fra. I nogle tilfælde kan det være nødvendigt at slette et af de objekter, der er i konflikt.
    
4. Hvis du har foretaget ændringen i den lokale AD, skal du lade Azure AD Forbind synkronisere ændringen, så fejlen bliver rettet.
    

