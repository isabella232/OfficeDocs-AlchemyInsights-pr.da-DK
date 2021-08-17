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
ms.openlocfilehash: 9b5765ff3c59b1312bead41a45a53478a96260df0567f006ab93c3ccfaf4be64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044334"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>KonsistensGuid/kildeAnchor-funktionsmåde

Azure AD Forbind (version 1.1.524.0 og nyere) letter nu brugen af msDS-ConsistencyGuid som kildeAnchor-attribut. Når du bruger denne funktion, konfigurerer Azure AD Forbind automatisk synkroniseringsregler til:
  
- Brug msDS-ConsistencyGuid som kildeAnchor-attributten for brugerobjekter. ObjectGUID bruges til andre objekttyper.
    
- For et givent lokalt AD User-objekt, hvis msDS-ConsistencyGuid-attribut ikke er udfyldt, skriver Azure AD Forbind dens objektGUID-værdi tilbage til attributten msDS-ConsistencyGuid i det lokale Active Directory. Når attributten msDS-ConsistencyGuid er udfyldt, eksporterer Azure AD Forbind objektet til Azure AD.
    
 **Bemærk!** Når et lokalt AD-objekt er importeret til Azure AD Forbind (dvs. importeret i AD-forbindelsesrummet og projiceret ind i Metaverse), kan du ikke længere ændre dens kildeanchor-værdi. Hvis du vil angive sourceAnchor-værdien for et givet lokalt AD-objekt, skal du konfigurere dens msDS-ConsistencyGuid-attribut, før den importeres til Azure AD Forbind. 
  
Du kan finde flere oplysninger om SourceAnchor og ConsistencyGuid i følgende: [Azure AD Forbind: Designkoncepter](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

