---
title: Fejl AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 5ac56fa78c66cf3b246bc0cc01f040e27310d629
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/18/2019
ms.locfileid: "36526977"
---
# <a name="error-attributevaluemustbeunique"></a>Fejl: AttributeValueMustBeUnique

Den mest almindelige årsag til AttributeValueMustBeUnique-fejlen er to objekter med forskelligt SourceAnchor (immutableId) med samme værdi for attributterne ProxyAddresses og/eller UserPrincipalName. Sådan rettes AttributeValueMustBeUnique-fejlen:
  
1. Identificer de duplikerede proxyadresser, userPrincipalName eller en anden attributværdi, der forårsager fejlen. Identificer også, hvilke to (eller flere) objekter der er involveret i konflikten. Den rapport, der genereres af Azure AD Connect Health for Sync, kan hjælpe dig med at identificere de to objekter.
    
2. Identificer, hvilket objekt der skal fortsætte med at have den duplikerede værdi, og hvilket objekt der ikke skal.
    
3. Fjern den duplikerede værdi fra det objekt, der ikke skal have den pågældende værdi. Bemærk, at du skal foretage ændringen i den mappe, hvor objektet stammer fra. I nogle tilfælde kan det være nødvendigt at slette et af objekterne i konflikt.
    
4. Hvis du foretog ændringen i den lokale annonce, skal du lade Azure AD Connect synkronisere ændringen, så fejlen bliver rettet.
    

