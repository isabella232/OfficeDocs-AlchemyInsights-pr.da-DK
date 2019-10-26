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
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/25/2019
ms.locfileid: "36516969"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="26171-102">Funktionsmåde for vilkÃ ¥/Sourceanker</span><span class="sxs-lookup"><span data-stu-id="26171-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="26171-103">Azure AD Connect (version 1.1.524.0 og After) gør det nu nemmere at bruge msDS--sammen-GUID som sourceAnchor-attribut.</span><span class="sxs-lookup"><span data-stu-id="26171-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="26171-104">Når du bruger denne funktion, konfigurerer Azure AD Connect automatisk synkroniserings reglerne til at:</span><span class="sxs-lookup"><span data-stu-id="26171-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="26171-105">Brug msDS-i-objekt-objektguid som sourceAnchor-attribut for bruger objekter.</span><span class="sxs-lookup"><span data-stu-id="26171-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="26171-106">ObjectGUID bruges til andre objekttyper.</span><span class="sxs-lookup"><span data-stu-id="26171-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="26171-107">I forbindelse med et lokalt AD User-objekt, hvis msDS-konsekvent-GUID-attribut ikke er udfyldt, skriver Azure AD Connect sin objectGUID-værdi tilbage til attributten msDS-sammen-Objekguid i Active Directory i det lokale miljø.</span><span class="sxs-lookup"><span data-stu-id="26171-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="26171-108">Når attributten msDS-sammen-objektguid er udfyldt, eksporterer Azure AD Connect derefter objektet til Azure AD.</span><span class="sxs-lookup"><span data-stu-id="26171-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="26171-109">**Bemærk:** Når et annonce objekt i det lokale miljø importeres til Azure AD Connect (som importeres til AD Connector-pladsen og projiceres til metaverse), kan du ikke længere ændre dets sourceAnchor-værdi.</span><span class="sxs-lookup"><span data-stu-id="26171-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="26171-110">Hvis du vil angive sourceAnchor-værdien for et givent annonce objekt i det lokale miljø, skal du konfigurere dens msDS-sammen-objektguid-attribut, før den importeres til Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="26171-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="26171-111">Du finder flere oplysninger om SourceAnchor og Vilkencyguid i følgende: [Azure ad Connect: design koncepter](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="26171-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

