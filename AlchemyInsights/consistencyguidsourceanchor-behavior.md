---
title: Konsistens- /kildeForankre-funktionsmåde
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
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 8527e7c2404742a999041f85ed12d78c48cc0d8c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705727"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>Konsistens- /kildeForankre-funktionsmåde

Azure AD Connect (version 1.1.524.0 og derefter) letter nu brugen af attributten msDS-ConsistencyGuid som kildeanker. Når du bruger denne funktion, konfigurerer Azure AD Connect automatisk synkroniseringsreglerne til:
  
- Brug msDS-KonsistensGuid som kildeAnkerattribut for Brugerobjekter. ObjectGUID bruges til andre objekttyper.
    
- For et givet lokalt AD-brugerobjekt, hvis msDS-ConsistencyGuid-attribut ikke er udfyldt, skriver Azure AD Connect sin objectGUID-værdi tilbage til attributten msDS-ConsistencyGuid i det lokale Active Directory. Når attributten msDS-ConsistencyGuid er udfyldt, eksporterer Azure AD Connect derefter objektet til Azure AD.
    
 **Bemærk:** Når et lokalt AD-objekt er importeret til Azure AD Connect (dvs. importeret til AD Connector Space og projiceret ind i Metaverse), kan du ikke længere ændre kildenS kildeAnkerværdi. Hvis du vil angive kildeankerværdien for et givet lokalt AD-objekt, skal du konfigurere attributten msDS-ConsistencyGuid, før den importeres til Azure AD Connect. 
  
Du kan finde flere oplysninger om SourceAnchor og ConsistencyGuid i følgende: [Azure AD Connect: Designkoncepter](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

