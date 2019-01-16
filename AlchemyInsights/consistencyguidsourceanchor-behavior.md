---
title: ConsistencyGuid / sourceAnchor funktionsmåde
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 80516ed9e15040475a8b65a1af98a1b561704d49
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/15/2019
ms.locfileid: "28282584"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor funktionsmåde

Azure AD Connect (version 1.1.524.0 og efter) nu letter brugen af msDS-ConsistencyGuid som sourceAnchor-attribut. Når du bruger denne funktion, konfigurerer Azure AD Connect automatisk synkronisering regler:
  
- Brug msDS-ConsistencyGuid som attributten sourceAnchor til brugerobjekter. ObjectGUID bruges til andre objekttyper.
    
- For ethvert givet lokale AD-bruger objektet hvis msDS-ConsistencyGuid-attribut ikke er udfyldt, Azure Connect AD skriver værdien objectGUID tilbage til attributten msDS-ConsistencyGuid i den lokale Active Directory. Når attributten msDS-ConsistencyGuid er udfyldt, eksporterer Azure AD Tilslut derefter objektet til Azure AD.
    
 **Bemærk:** Når en lokal AD objektet indlæses i Azure AD Connect (der er importeret til AD Connector-plads og forventet i Metaverse), du kan ikke ændre dens værdi til sourceAnchor længere. Angive sourceAnchor-værdi for en givet lokale AD objekt, konfigurere sin msDS-ConsistencyGuid-attribut, før den importeres til Azure AD Connect. 
  
Yderligere oplysninger om SourceAnchor og ConsistencyGuid, henvises til følgende: [Azure AD Connect: Design begreber](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

