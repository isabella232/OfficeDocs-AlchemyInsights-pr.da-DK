---
title: FejlattributtenValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: fa1fdb35f1af250bc98aa61c0e5111f1f1b8aac4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703168"
---
# <a name="error-attributevaluemustbeunique"></a>Fejl: AttributValueMustBeUnique

Den mest almindelige årsag til fejlen AttributValueMustBeUnique er, at to objekter med forskellige SourceAnchor-attributter (immutableId) har samme værdi for proxyadresser og/eller UserPrincipalName-attributter. Sådan rettes fejlen AttributValueMustBeUnique:
  
1. Identificer de dublerede proxyadresser, userPrincipalName eller en anden attributværdi, der forårsager fejlen. Angiv også, hvilke to (eller flere) objekter der er involveret i konflikten. Den rapport, der genereres af Azure AD Connect Health til synkronisering, kan hjælpe dig med at identificere de to objekter.
    
2. Identificer, hvilket objekt der fortsat skal have den duplikerede værdi, og hvilket objekt der ikke skal.
    
3. Fjern den duplikerede værdi fra objektet, der IKKE bør have denne værdi. Bemærk, at du skal foretage ændringen i den mappe, hvor objektet stammer fra. I nogle tilfælde skal du muligvis slette et af objekterne i konflikt.
    
4. Hvis du har foretaget ændringen i den lokale AD, skal du lade Azure AD Connect synkronisere ændringen, så fejlen bliver rettet.
    

