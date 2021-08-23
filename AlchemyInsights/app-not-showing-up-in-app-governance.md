---
title: Min app vises ikke i Appstyring
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12734"
ms.openlocfilehash: a8d176fdee073e41b61de6f53c728601da955aaa
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/16/2021
ms.locfileid: "58454540"
---
# <a name="my-app-isnt-showing-up-in-app-governance"></a>Min app vises ikke i Appstyring

Hvis programmet ikke vises under Appstyring, skal du kontrollere følgende:

1. Gå til [Azure AD,](https://aad.portal.azure.com/) og find app-id'et for dit program ved at søge efter navnet på appen i den øverste linje på siden Oversigt.

1. Access Graph Stifinder, og søg efter app-id'et i din tjeneste principal ved hjælp af denne forespørgsel og erstatter med det <appId> relevante app-id: < https://graph.microsoft.com/v1.0/servicePrincipals? $search = "appId: <appId> ">

1. Hvis der ikke returneres nogen resultater, kan du søge efter app-id'et i programmet ved hjælp af denne forespørgsel og erstatte med det relevante <appId> app-id: < https://graph.microsoft.com/v1.0/applications? $search = "appId: <appId> ">

Hvis du oplever problemer med forespørgslen, skal du se [Få support](https://docs.microsoft.com/microsoft-365/business-video/get-help-support). 

Du kan finde flere oplysninger eller indsigt i dine apps i Appstyring i [Få mere at vide om synlighed og indsigt](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-overview).

Du kan finde flere oplysninger om visning af dine apps under [Få vist dine apps](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-view-apps).
