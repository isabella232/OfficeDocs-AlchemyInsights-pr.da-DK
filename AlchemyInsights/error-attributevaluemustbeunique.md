---
title: Fejl AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7a97d1a5ff352b55833bd457e3220a56130d7e7e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499628"
---
# <a name="error-attributevaluemustbeunique"></a>Fejl: AttributeValueMustBeUnique

Den mest almindelige årsag til fejlen AttributeValueMustBeUnique er to objekter med forskellige SourceAnchor (immutableId) har samme værdi for attributterne ProxyAddresses og/eller UserPrincipalName. Rette fejlen AttributeValueMustBeUnique:
  
1. Identificere identiske proxyAddresses, userPrincipalName eller andre-attributværdi, der er årsag til fejlen. Også identificere, hvilke to (eller flere) objekter, der er involveret i konflikten. Den rapport, der er genereret af Azure AD forbinde sundhed for synkronisering kan hjælpe dig med at identificere de to objekter.
    
2. Identificere, hvilket objekt der bør fortsat have den identiske værdi, og hvilket objekt må ikke.
    
3. Fjern den identiske værdi fra det objekt, der ikke skal have værdien. Bemærk, at du skal foretage ændringen i den mappe, hvor objektet er leveres fra. I nogle tilfælde skal du slette et af objekterne i konflikt.
    
4. Hvis du har foretaget ændringen i lokaler på Annoncen, Lad Azure AD Connect synkronisere ændringen at få rettet fejlen.
    

