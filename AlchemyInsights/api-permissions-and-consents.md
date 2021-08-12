---
title: API-tilladelser og -samtykke
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
ms.openlocfilehash: c45bab67d414c8f0f2ca1c5275084d4ecce538c5256154292302080ba5bd8175
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932091"
---
# <a name="api-permissions-and-consent"></a>API-tilladelser og samtykke

Programmer, der integreres med Microsoft-identitetsplatform en godkendelsesmodel, der giver brugere og administratorer kontrol over, hvordan data kan tilgås. Implementeringen af godkendelsesmodellen er blevet opdateret Microsoft-identitetsplatform slutpunktet. Den ændrer, hvordan en app skal interagere med Microsoft-identitetsplatform. [Tilladelser og samtykke i Microsoft-identitetsplatform dækker](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) de grundlæggende begreber i denne godkendelsesmodel, herunder omfang, tilladelser og samtykke.

[Tilladelsesrammen Azure Active Directory Azure AD (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) gør det nemt at udvikle webprogrammer med flere lejere og oprindelige klientprogrammer. Disse programmer tillader logon af brugerkonti fra en Azure AD-lejer, der er forskellig fra den, hvor programmet er registreret. De skal muligvis også have adgang til web-API'er som f.eks. Microsoft Graph API (for at få adgang til Azure AD, Intune og tjenester i Microsoft 365) og andre Microsoft-tjenester' API'er ud over dine egne web-API'er.

