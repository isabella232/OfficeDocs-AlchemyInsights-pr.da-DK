---
title: Problemer med administratortilladelse
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900928"
---
# <a name="admin-consent-issues"></a>Problemer med administratortilladelse

1. Aktivere [arbejdsgangen for administrator samtykke](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) for at give brugerne mulighed for at anmode om administratorgodkendelse direkte fra samtykke skærmen.

1. Hvis du eller dit programs brugere får uventede fejl under tilladelses processen, skal du læse denne artikel for at få fejlfindingstrin: [uventet fejl, når du udfører et samtykke til et program](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).

1. Få mere at vide om [administrator samtykke på Microsoft Identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), hvordan [samtykkes meddelelsen](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) fungerer, og hvordan du [evaluerer en anmodning om administratortilladelse i hele lejeren](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).

1. Programmer, der integreres med Microsoft Identity platform, følger en godkendelsesmodel, der giver brugere og administratorer kontrol over, hvordan data kan åbnes. Implementeringen af godkendelses modellen er blevet opdateret på Microsoft Identity platform Endpoint, og det ændrer, hvordan en app skal interagere med Microsoft Identity platform. Se [tilladelser og samtykke i Microsoft Identity platform Endpoint for at](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) få en oversigt over denne godkendelsesmodel, herunder områder, tilladelser og samtykke.