---
title: ConsistencyGuid/sourceAnchor-opførsel
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
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: adac469328485696d1ee1532aa3d6828af0642eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756277"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor-opførsel

Azure AD Connect (version 1.1.524.0 og After) gør det nu nemmere at bruge attributten msDS-ConsistencyGuid som sourceAnchor-attribut. Når du bruger denne funktion, konfigurerer Azure AD Connect automatisk synkroniseringsreglerne til:
  
- Brug attributten msDS-ConsistencyGuid som sourceAnchor-attribut for bruger objekter. ObjectGUID bruges til andre objekttyper.
    
- I forbindelse med et givet lokalt brugerobjekt, hvor attributten msDS-ConsistencyGuid ikke er udfyldt, skriver Azure AD Connect sin objectGUID-værdi tilbage til attributten msDS-ConsistencyGuid i Active Directory lokalt. Når attributten msDS-ConsistencyGuid er udfyldt, eksporterer Azure AD Connect derefter objektet til Azure AD.
    
 **Bemærk:** Når et lokalt AD-objekt importeres til Azure AD Connect (dvs. importeret til AD-forbindelses pladsen og projiceres ind i Metaverse), kan du ikke længere ændre sin sourceAnchor-værdi. Hvis du vil angive sourceAnchor-værdien for et givet lokalt AD-objekt, skal du konfigurere attributten msDS-ConsistencyGuid, før den importeres til Azure AD Connect. 
  
Hvis du vil have mere at vide om SourceAnchor og ConsistencyGuid, skal du se følgende: [Azure ad Connect: design koncepter](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

