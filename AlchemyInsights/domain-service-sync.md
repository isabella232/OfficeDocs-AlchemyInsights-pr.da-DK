---
title: Synkronisering af domæne tjeneste
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.openlocfilehash: b35d3a402bc08a27a818209385c5666b901fa524
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/15/2021
ms.locfileid: "49884956"
---
# <a name="domain-service-synchronization"></a><span data-ttu-id="d835a-102">Synkronisering af domæne tjeneste</span><span class="sxs-lookup"><span data-stu-id="d835a-102">Domain service synchronization</span></span>

<span data-ttu-id="d835a-103">Objekter og legitimationsoplysninger i et Azure Active Directory Domain Services (Azure AD DS)-administreret domæne kan enten oprettes lokalt inden for domænet eller synkroniseres fra en Azure Active Directory-lejer (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="d835a-103">Objects and credentials in an Azure Active Directory Domain Services (Azure AD DS) managed domain can either be created locally within the domain, or synchronized from an Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="d835a-104">Når du første gang installerer Azure AD DS, konfigureres og startes en automatisk envejs synkronisering for at replikere objekterne fra Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d835a-104">When you first deploy Azure AD DS, an automatic one-way synchronization is configured and initiated to replicate the objects from Azure AD.</span></span> <span data-ttu-id="d835a-105">Denne envejs synkronisering kører fortsat i baggrunden for at holde Azure AD DS Managed-domænet opdateret med eventuelle ændringer fra Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d835a-105">This one-way synchronization continues to run in the background to keep the Azure AD DS managed domain up-to-date with any changes from Azure AD.</span></span> <span data-ttu-id="d835a-106">Der sker ingen synkronisering fra Azure AD DS tilbage til Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d835a-106">No synchronization occurs from Azure AD DS back to Azure AD.</span></span>

<span data-ttu-id="d835a-107">Du kan få mere at vide om synkronisering af Active Directory-domæne tjenester i Azure, under [synkronisering af domæne tjeneste](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span><span class="sxs-lookup"><span data-stu-id="d835a-107">For more details on Azure Active Directory domain service synchronization, see [Domain Service Synchronization](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span></span> 
