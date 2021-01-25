---
title: API-tilladelser og-samtykke
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974371"
---
# <a name="api-permissions-and-consent"></a>API-tilladelser og-samtykke

Programmer, der integreres med Microsoft Identity platform, følger en godkendelsesmodel, der giver brugere og administratorer kontrol over, hvordan data kan åbnes. Implementeringen af godkendelses modellen er blevet opdateret på Microsoft Identity platform Endpoint. Det ændrer, hvordan en app skal interagere med Microsoft Identity platform. [Tilladelser og samtykke i Microsoft Identity platform Endpoint](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) dækker de grundlæggende begreber for denne godkendelsesmodel, herunder områder, tilladelser og samtykke.

[Azure Active Directory (Azure ad)-samtykke Framework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) gør det nemt at udvikle Internet-og oprindelige klientprogrammer fra flere arkitekturer. Disse programmer tillader, at der logges af brugerkonti fra en Azure AD-lejer, der er anderledes end den, hvor programmet er registreret. De kan også have brug for at få adgang til webapi'er som Microsoft Graph API (for at få adgang til Azure AD, Intune og tjenester i Microsoft 365) og andre Microsoft-tjenesters API'er, ud over dine egne webapi'er.

