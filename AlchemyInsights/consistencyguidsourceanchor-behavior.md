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
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="b8076-102">ConsistencyGuid / sourceAnchor funktionsmåde</span><span class="sxs-lookup"><span data-stu-id="b8076-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="b8076-103">Azure AD Connect (version 1.1.524.0 og efter) nu letter brugen af msDS-ConsistencyGuid som sourceAnchor-attribut.</span><span class="sxs-lookup"><span data-stu-id="b8076-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="b8076-104">Når du bruger denne funktion, konfigurerer Azure AD Connect automatisk synkronisering regler:</span><span class="sxs-lookup"><span data-stu-id="b8076-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="b8076-105">Brug msDS-ConsistencyGuid som attributten sourceAnchor til brugerobjekter.</span><span class="sxs-lookup"><span data-stu-id="b8076-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="b8076-106">ObjectGUID bruges til andre objekttyper.</span><span class="sxs-lookup"><span data-stu-id="b8076-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="b8076-107">For ethvert givet lokale AD-bruger objektet hvis msDS-ConsistencyGuid-attribut ikke er udfyldt, Azure Connect AD skriver værdien objectGUID tilbage til attributten msDS-ConsistencyGuid i den lokale Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b8076-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="b8076-108">Når attributten msDS-ConsistencyGuid er udfyldt, eksporterer Azure AD Tilslut derefter objektet til Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b8076-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="b8076-109">**Bemærk:** Når en lokal AD objektet indlæses i Azure AD Connect (der er importeret til AD Connector-plads og forventet i Metaverse), du kan ikke ændre dens værdi til sourceAnchor længere.</span><span class="sxs-lookup"><span data-stu-id="b8076-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="b8076-110">Angive sourceAnchor-værdi for en givet lokale AD objekt, konfigurere sin msDS-ConsistencyGuid-attribut, før den importeres til Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="b8076-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="b8076-111">Yderligere oplysninger om SourceAnchor og ConsistencyGuid, henvises til følgende: [Azure AD Connect: Design begreber](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="b8076-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

