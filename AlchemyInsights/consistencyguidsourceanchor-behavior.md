---
title: ConsistencyGuid / sourceAnchor funktionsmåde
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: cb1b50792b07a1b3b69607bf2f6824141a15922f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/23/2019
ms.locfileid: "32408102"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor funktionsmåde

Azure AD Connect (version 1.1.524.0 og efter) nu letter brugen af msDS-ConsistencyGuid som sourceAnchor-attribut. Når du bruger denne funktion, konfigurerer Azure AD Connect automatisk synkronisering regler:
  
- Brug msDS-ConsistencyGuid som attributten sourceAnchor til brugerobjekter. ObjectGUID bruges til andre objekttyper.
    
- For ethvert givet lokale AD-bruger objektet hvis msDS-ConsistencyGuid-attribut ikke er udfyldt, Azure Connect AD skriver værdien objectGUID tilbage til attributten msDS-ConsistencyGuid i den lokale Active Directory. Når attributten msDS-ConsistencyGuid er udfyldt, eksporterer Azure AD Tilslut derefter objektet til Azure AD.
    
 **Bemærk:** Når en lokal AD objektet indlæses i Azure AD Connect (der er importeret til AD Connector-plads og forventet i Metaverse), du kan ikke ændre dens værdi til sourceAnchor længere. Angive sourceAnchor-værdi for en givet lokale AD objekt, konfigurere sin msDS-ConsistencyGuid-attribut, før den importeres til Azure AD Connect. 
  
Yderligere oplysninger om SourceAnchor og ConsistencyGuid, henvises til følgende: [Azure AD Connect: Design begreber](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

