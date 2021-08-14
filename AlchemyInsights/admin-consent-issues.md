---
title: Problemer med administratorsamtykke
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
ms.openlocfilehash: 08d3bfa84fd5ab31d7165090c392866d863898545ade7631e820a100eef89dea
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952567"
---
# <a name="admin-consent-issues"></a>Problemer med administratorsamtykke

1. Aktivér [arbejdsprocessen for administratorsamtykke](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) for at give brugere mulighed for at anmode om administratorgodkendelse direkte fra skærmen med samtykke.

1. Hvis du eller dit programs brugere får vist uventede fejl under samtykkeprocessen, kan du læse denne artikel for at få fejlfindingstrin: Uventet fejl, når du udfører samtykke [til et program.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)

1. Få mere at vide [om administratorsamtykke på](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)Microsoft-identitetsplatform, hvordan samtykkeprompten fungerer, og hvordan du evaluerer en anmodning om [administratorsamtykke for hele lejeren.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) [](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)

1. Programmer, der integreres med Microsoft-identitetsplatform en godkendelsesmodel, der giver brugere og administratorer kontrol over, hvordan data kan tilgås. Implementeringen af godkendelsesmodellen er blevet opdateret på Microsoft-identitetsplatform slutpunktet, og det ændrer, hvordan en app skal interagere med Microsoft-identitetsplatform. Se [Tilladelser og samtykke i Microsoft-identitetsplatform for](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) at få en oversigt over denne godkendelsesmodel, herunder omfang, tilladelser og samtykke.