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
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="dfa8d-102">ConsistencyGuid/sourceAnchor-opførsel</span><span class="sxs-lookup"><span data-stu-id="dfa8d-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="dfa8d-103">Azure AD Connect (version 1.1.524.0 og After) gør det nu nemmere at bruge attributten msDS-ConsistencyGuid som sourceAnchor-attribut.</span><span class="sxs-lookup"><span data-stu-id="dfa8d-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="dfa8d-104">Når du bruger denne funktion, konfigurerer Azure AD Connect automatisk synkroniseringsreglerne til:</span><span class="sxs-lookup"><span data-stu-id="dfa8d-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="dfa8d-105">Brug attributten msDS-ConsistencyGuid som sourceAnchor-attribut for bruger objekter.</span><span class="sxs-lookup"><span data-stu-id="dfa8d-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="dfa8d-106">ObjectGUID bruges til andre objekttyper.</span><span class="sxs-lookup"><span data-stu-id="dfa8d-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="dfa8d-107">I forbindelse med et givet lokalt brugerobjekt, hvor attributten msDS-ConsistencyGuid ikke er udfyldt, skriver Azure AD Connect sin objectGUID-værdi tilbage til attributten msDS-ConsistencyGuid i Active Directory lokalt.</span><span class="sxs-lookup"><span data-stu-id="dfa8d-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="dfa8d-108">Når attributten msDS-ConsistencyGuid er udfyldt, eksporterer Azure AD Connect derefter objektet til Azure AD.</span><span class="sxs-lookup"><span data-stu-id="dfa8d-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="dfa8d-109">**Bemærk:** Når et lokalt AD-objekt importeres til Azure AD Connect (dvs. importeret til AD-forbindelses pladsen og projiceres ind i Metaverse), kan du ikke længere ændre sin sourceAnchor-værdi.</span><span class="sxs-lookup"><span data-stu-id="dfa8d-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="dfa8d-110">Hvis du vil angive sourceAnchor-værdien for et givet lokalt AD-objekt, skal du konfigurere attributten msDS-ConsistencyGuid, før den importeres til Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="dfa8d-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="dfa8d-111">Hvis du vil have mere at vide om SourceAnchor og ConsistencyGuid, skal du se følgende: [Azure ad Connect: design koncepter](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="dfa8d-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

