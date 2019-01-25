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
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/24/2019
ms.locfileid: "29498512"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="0c57f-102">ConsistencyGuid / sourceAnchor funktionsmåde</span><span class="sxs-lookup"><span data-stu-id="0c57f-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="0c57f-p101">Azure AD Connect (version 1.1.524.0 og efter) nu letter brugen af msDS-ConsistencyGuid som sourceAnchor-attribut. Når du bruger denne funktion, konfigurerer Azure AD Connect automatisk synkronisering regler:</span><span class="sxs-lookup"><span data-stu-id="0c57f-p101">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute. When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="0c57f-p102">Brug msDS-ConsistencyGuid som attributten sourceAnchor til brugerobjekter. ObjectGUID bruges til andre objekttyper.</span><span class="sxs-lookup"><span data-stu-id="0c57f-p102">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects. ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="0c57f-p103">For ethvert givet lokale AD-bruger objektet hvis msDS-ConsistencyGuid-attribut ikke er udfyldt, Azure Connect AD skriver værdien objectGUID tilbage til attributten msDS-ConsistencyGuid i den lokale Active Directory. Når attributten msDS-ConsistencyGuid er udfyldt, eksporterer Azure AD Tilslut derefter objektet til Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0c57f-p103">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory. After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="0c57f-p104">**Bemærk:** Når en lokal AD objektet indlæses i Azure AD Connect (der er importeret til AD Connector-plads og forventet i Metaverse), du kan ikke ændre dens værdi til sourceAnchor længere. Angive sourceAnchor-værdi for en givet lokale AD objekt, konfigurere sin msDS-ConsistencyGuid-attribut, før den importeres til Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="0c57f-p104">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore. To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="0c57f-111">Yderligere oplysninger om SourceAnchor og ConsistencyGuid, henvises til følgende: [Azure AD Connect: Design begreber](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="0c57f-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

