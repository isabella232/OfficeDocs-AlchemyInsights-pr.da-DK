---
title: API-tilladelser og samtykkeproces
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "9200"
ms.openlocfilehash: 078f5798533dfbbf97858f305729f103663644fee3590cdcc877233041adae81
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932055"
---
# <a name="api-permissions-and-consent-process"></a>API-tilladelser og samtykkeproces

Hvis din app skal have adgang til data i Microsoft Graph, skal brugeren eller administratoren give den de rette tilladelser via en samtykkeproces. [Microsoft Graph tilladelsesreferencer viser](https://docs.microsoft.com/graph/permissions-reference) de tilladelser, der er knyttet til hvert overordnede sæt af Microsoft-Graph API'er. Den indeholder også vejledning til, hvordan du bruger tilladelserne.

**Konfigurer eller opdater tjenesteinspektør**

- [Opret serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) – I denne artikel kan du se, hvordan du opretter et nyt servicePrincipal-objekt.
- [Opret en Azure AD-app](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) &-tjenesteinspektør på portalen – Denne artikel viser, hvordan du opretter et nyt Azure Active Directory-program (Azure AD) og tjenesteinspektør, der kan bruges med det rollebaserede adgangskontrolelement.
- [Apps](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) &-tjenesteinspektører i Azure AD – I denne artikel beskrives programregistrering, programobjekter og tjenesteinspektører i Azure Active Directory: hvad de er, hvordan de bruges, og hvordan de er relateret til hinanden.

**Tilføje eller opdatere appregistrering og give administratorsamtykke**

- [Oprette en appregistrering –](https://docs.microsoft.com/graph/api/application-post-applications) I denne artikel kan du se, hvordan du opretter et nyt programobjekt.
- [Opdatere en appregistrering – API-tilladelser](https://docs.microsoft.com/graph/api/application-update) – Denne artikel viser, hvordan du opdaterer egenskaberne for et programobjekt.
- [Giv administratorsamtykke](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) – For administratorsamtykke og samtykke generelt kræver vi, at en administrator udtrykkeligt giver samtykke.
- [RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) – Beholder til rollestyring for samlede rolledefinitioner og rolletildelinger for Microsoft 365 RBAC-udbydere, der understøtter flere hovedstole og flere områder i en enkelt rolletildeling. Dette er forskelligt fra *rbacApplication-ressourcetype.* Microsoft Intune er et eksempel på en sådan RBAC-udbyder. En rolletildeling i Intune kan have en matrix med hovedstole og en matrix med omfangsgrupper. **Dette er i betaversionen, hvilket betyder, at den stadig er under udvikling og ikke anbefales til brug i produktion.**
