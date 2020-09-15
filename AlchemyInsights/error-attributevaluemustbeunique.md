---
title: Fejl AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 4627a7ae34b0dd9f16538ef75ac8792672dcc056
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709145"
---
# <a name="error-attributevaluemustbeunique"></a>Fejl: AttributeValueMustBeUnique

Den mest almindelige årsag til AttributeValueMustBeUnique-fejlen er to objekter med forskellige SourceAnchor (immutableId), der har samme værdi for ProxyAddresses-og/eller UserPrincipalName-attributterne. Sådan retter du fejlen AttributeValueMustBeUnique:
  
1. Identificer den duplikerede proxyAddresses, userPrincipalName eller anden attributværdi, der forårsager fejlen. Identificer også, hvilke to (eller flere) objekter der er involveret i konflikten. Rapporten, der er oprettet af Azure AD Connect-tilstand for Sync, kan hjælpe dig med at identificere de to objekter.
    
2. Identificer, hvilket objekt der skal fortsætte med at have den duplikerede værdi, og hvilket objekt bør ikke.
    
3. Fjern den duplikerede værdi fra det objekt, der ikke skal have den værdi. Bemærk, at du skal udføre ændringen i den mappe, hvor objektet er kildet fra. I nogle tilfælde kan det være nødvendigt at slette et af de objekter, der er i konflikt.
    
4. Hvis du har foretaget ændringen i REKLAMEn på stedet, skal du lade Azure AD Connect synkronisere ændringen for at få løst fejlen.
    

