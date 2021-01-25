---
title: Attributtilknytning af brugerklargøring
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949697"
---
# <a name="user-provisioning-attribute-mapping"></a><span data-ttu-id="ae635-102">Attributtilknytning af brugerklargøring</span><span class="sxs-lookup"><span data-stu-id="ae635-102">User-provisioning attribute mapping</span></span>

1. <span data-ttu-id="ae635-103">Hvis du vil foretage fejlfinding af kendte attribut tilknytnings problemer, skal du se [attributtilknytninger](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span><span class="sxs-lookup"><span data-stu-id="ae635-103">To troubleshoot known attribute-mapping issues, see [Attribute mappings](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span></span> 
2. <span data-ttu-id="ae635-104">Microsoft Azure Active Directory (AD) yder support til brugerklargøring til tredjeparts SaaS-programmer som Salesforce, G Suite og andre.</span><span class="sxs-lookup"><span data-stu-id="ae635-104">Microsoft Azure Active Directory (AD) provides support for user provisioning to third-party SaaS applications such as Salesforce, G Suite and others.</span></span> <span data-ttu-id="ae635-105">Hvis du aktiverer brugerklargøring for et tredjeparts SaaS-program, styrer Azure-portalen dens attributværdier via attributtilknytninger.</span><span class="sxs-lookup"><span data-stu-id="ae635-105">If you enable user provisioning for a third-party SaaS application, the Azure portal controls its attribute values through attribute-mappings.</span></span> <span data-ttu-id="ae635-106">Du kan få mere at vide om, hvordan du tilpasser standardattribut tilknytninger, under [Tilpas bruger klargørings attribut-tilknytninger for SaaS-programmer i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span><span class="sxs-lookup"><span data-stu-id="ae635-106">To learn how to customize the default attribute-mappings, see [Customize user provisioning attribute-mappings for SaaS applications in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span></span>
    - <span data-ttu-id="ae635-107">Hvis du vil have mere at vide om SaaS app user provisions, skal du se [Hvad er provisions klargøring af-appen i Azure ad?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span><span class="sxs-lookup"><span data-stu-id="ae635-107">To learn more about SaaS app user provisioning, see [What is automated SaaS app user provisioning in Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span></span> 
3. <span data-ttu-id="ae635-108">Når du tilpasser attribut-tilknytninger for brugerklargøring, kan du finde ud af, at den attribut, du vil tilknytte, ikke vises på listen kildeattribut.</span><span class="sxs-lookup"><span data-stu-id="ae635-108">When customizing attribute-mappings for user provisioning, you might find that the attribute you want to map doesn't appear in the Source attribute list.</span></span> <span data-ttu-id="ae635-109">[Attributten Synkroniser en attribut fra dit lokale Active Directory til Azure ad for at blive klargjort til en program](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) artikel viser dig, hvordan du tilføjer den manglende attribut ved at synkronisere den fra din lokale ad til Azure ad.</span><span class="sxs-lookup"><span data-stu-id="ae635-109">The [Sync an attribute from your on-premises Active Directory to Azure AD for provisioning to an application](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) article shows you how to add the missing attribute by synchronizing it from your on-premises AD to Azure AD.</span></span>
