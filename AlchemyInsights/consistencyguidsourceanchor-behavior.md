---
title: KonsistensGuid/kildeAnchor-funktionsmåde
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
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: eafe1ec9636cddc9d73a88beb7ae3ad9f6fad660
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816986"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>KonsistensGuid/kildeAnchor-funktionsmåde

Azure AD Connect (version 1.1.524.0 og nyere) letter nu brugen af msDS-ConsistencyGuid som kildeAnchor-attribut. Når du bruger denne funktion, konfigurerer Azure AD Connect automatisk synkroniseringsregler til:
  
- Brug msDS-ConsistencyGuid som kildeAnchor-attributten for brugerobjekter. ObjectGUID bruges til andre objekttyper.
    
- For et givent lokalt AD User-objekt, hvis msDS-ConsistencyGuid-attribut ikke er udfyldt, skriver Azure AD Connect dens objektGUID-værdi tilbage til attributten msDS-ConsistencyGuid i Active Directory i det lokale miljø. Når attributten msDS-ConsistencyGuid er udfyldt, eksporterer Azure AD Connect derefter objektet til Azure AD.
    
 **Bemærk!** Når et lokalt AD-objekt er importeret til Azure AD Connect (dvs. importeret til AD-forbindelsesrummet og projiceret ind i Metaverse), kan du ikke længere ændre dens kildeværdi forAnchor. Hvis du vil angive sourceAnchor-værdien for et givet lokalt AD-objekt, skal du konfigurere dens msDS-ConsistencyGuid-attribut, før den importeres til Azure AD Connect. 
  
Du kan finde flere oplysninger om SourceAnchor og ConsistencyGuid i følgende: [Azure AD Connect: Designkoncepter](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

