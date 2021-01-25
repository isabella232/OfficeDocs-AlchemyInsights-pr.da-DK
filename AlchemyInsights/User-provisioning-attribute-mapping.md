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
# <a name="user-provisioning-attribute-mapping"></a>Attributtilknytning af brugerklargøring

1. Hvis du vil foretage fejlfinding af kendte attribut tilknytnings problemer, skal du se [attributtilknytninger](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings). 
2. Microsoft Azure Active Directory (AD) yder support til brugerklargøring til tredjeparts SaaS-programmer som Salesforce, G Suite og andre. Hvis du aktiverer brugerklargøring for et tredjeparts SaaS-program, styrer Azure-portalen dens attributværdier via attributtilknytninger. Du kan få mere at vide om, hvordan du tilpasser standardattribut tilknytninger, under [Tilpas bruger klargørings attribut-tilknytninger for SaaS-programmer i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).
    - Hvis du vil have mere at vide om SaaS app user provisions, skal du se [Hvad er provisions klargøring af-appen i Azure ad?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning) 
3. Når du tilpasser attribut-tilknytninger for brugerklargøring, kan du finde ud af, at den attribut, du vil tilknytte, ikke vises på listen kildeattribut. [Attributten Synkroniser en attribut fra dit lokale Active Directory til Azure ad for at blive klargjort til en program](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) artikel viser dig, hvordan du tilføjer den manglende attribut ved at synkronisere den fra din lokale ad til Azure ad.
