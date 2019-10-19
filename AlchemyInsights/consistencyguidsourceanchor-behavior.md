---
title: Funktionsmåde for vilkÃ ¥/Sourceanker
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
ms.openlocfilehash: f0ff94a8e46f1fb4e0ac8653c51f8f651e29498b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/18/2019
ms.locfileid: "36516969"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>Funktionsmåde for vilkÃ ¥/Sourceanker

Azure AD Connect (version 1.1.524.0 og After) gør det nu nemmere at bruge msDS--sammen-GUID som sourceAnchor-attribut. Når du bruger denne funktion, konfigurerer Azure AD Connect automatisk synkroniserings reglerne til at:
  
- Brug msDS-i-objekt-objektguid som sourceAnchor-attribut for bruger objekter. ObjectGUID bruges til andre objekttyper.
    
- I forbindelse med et lokalt AD User-objekt, hvis msDS-konsekvent-GUID-attribut ikke er udfyldt, skriver Azure AD Connect sin objectGUID-værdi tilbage til attributten msDS-sammen-Objekguid i Active Directory i det lokale miljø. Når attributten msDS-sammen-objektguid er udfyldt, eksporterer Azure AD Connect derefter objektet til Azure AD.
    
 **Bemærk:** Når et annonce objekt i det lokale miljø importeres til Azure AD Connect (som importeres til AD Connector-pladsen og projiceres til metaverse), kan du ikke længere ændre dets sourceAnchor-værdi. Hvis du vil angive sourceAnchor-værdien for et givent annonce objekt i det lokale miljø, skal du konfigurere dens msDS-sammen-objektguid-attribut, før den importeres til Azure AD Connect. 
  
Du finder flere oplysninger om SourceAnchor og Vilkencyguid i følgende: [Azure ad Connect: design koncepter](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

