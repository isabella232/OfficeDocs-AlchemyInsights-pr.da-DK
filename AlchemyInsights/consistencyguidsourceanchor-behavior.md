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
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="5696c-102">Konsistens- /kildeForankre-funktionsmåde</span><span class="sxs-lookup"><span data-stu-id="5696c-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="5696c-103">Azure AD Connect (version 1.1.524.0 og derefter) letter nu brugen af attributten msDS-ConsistencyGuid som kildeanker.</span><span class="sxs-lookup"><span data-stu-id="5696c-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="5696c-104">Når du bruger denne funktion, konfigurerer Azure AD Connect automatisk synkroniseringsreglerne til:</span><span class="sxs-lookup"><span data-stu-id="5696c-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="5696c-105">Brug msDS-KonsistensGuid som kildeAnkerattribut for Brugerobjekter.</span><span class="sxs-lookup"><span data-stu-id="5696c-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="5696c-106">ObjectGUID bruges til andre objekttyper.</span><span class="sxs-lookup"><span data-stu-id="5696c-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="5696c-107">For et givet lokalt AD-brugerobjekt, hvis msDS-ConsistencyGuid-attribut ikke er udfyldt, skriver Azure AD Connect sin objectGUID-værdi tilbage til attributten msDS-ConsistencyGuid i det lokale Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5696c-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="5696c-108">Når attributten msDS-ConsistencyGuid er udfyldt, eksporterer Azure AD Connect derefter objektet til Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5696c-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="5696c-109">**Bemærk:** Når et lokalt AD-objekt er importeret til Azure AD Connect (dvs. importeret til AD Connector Space og projiceret ind i Metaverse), kan du ikke længere ændre kildenS kildeAnkerværdi.</span><span class="sxs-lookup"><span data-stu-id="5696c-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="5696c-110">Hvis du vil angive kildeankerværdien for et givet lokalt AD-objekt, skal du konfigurere attributten msDS-ConsistencyGuid, før den importeres til Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="5696c-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="5696c-111">Du kan finde flere oplysninger om SourceAnchor og ConsistencyGuid i følgende: [Azure AD Connect: Designkoncepter](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="5696c-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

