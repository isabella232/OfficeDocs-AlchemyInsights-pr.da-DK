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
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="c7a55-102">KonsistensGuid/kildeAnchor-funktionsmåde</span><span class="sxs-lookup"><span data-stu-id="c7a55-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="c7a55-103">Azure AD Connect (version 1.1.524.0 og nyere) letter nu brugen af msDS-ConsistencyGuid som kildeAnchor-attribut.</span><span class="sxs-lookup"><span data-stu-id="c7a55-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="c7a55-104">Når du bruger denne funktion, konfigurerer Azure AD Connect automatisk synkroniseringsregler til:</span><span class="sxs-lookup"><span data-stu-id="c7a55-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="c7a55-105">Brug msDS-ConsistencyGuid som kildeAnchor-attributten for brugerobjekter.</span><span class="sxs-lookup"><span data-stu-id="c7a55-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="c7a55-106">ObjectGUID bruges til andre objekttyper.</span><span class="sxs-lookup"><span data-stu-id="c7a55-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="c7a55-107">For et givent lokalt AD User-objekt, hvis msDS-ConsistencyGuid-attribut ikke er udfyldt, skriver Azure AD Connect dens objektGUID-værdi tilbage til attributten msDS-ConsistencyGuid i Active Directory i det lokale miljø.</span><span class="sxs-lookup"><span data-stu-id="c7a55-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="c7a55-108">Når attributten msDS-ConsistencyGuid er udfyldt, eksporterer Azure AD Connect derefter objektet til Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c7a55-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="c7a55-109">**Bemærk!** Når et lokalt AD-objekt er importeret til Azure AD Connect (dvs. importeret til AD-forbindelsesrummet og projiceret ind i Metaverse), kan du ikke længere ændre dens kildeværdi forAnchor.</span><span class="sxs-lookup"><span data-stu-id="c7a55-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="c7a55-110">Hvis du vil angive sourceAnchor-værdien for et givet lokalt AD-objekt, skal du konfigurere dens msDS-ConsistencyGuid-attribut, før den importeres til Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="c7a55-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="c7a55-111">Du kan finde flere oplysninger om SourceAnchor og ConsistencyGuid i følgende: [Azure AD Connect: Designkoncepter](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="c7a55-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

