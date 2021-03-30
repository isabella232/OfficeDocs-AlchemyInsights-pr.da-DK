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
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/26/2021
ms.locfileid: "51404501"
---
# <a name="api-permissions-and-consent-process"></a>API-tilladelser og samtykkeproces

For at din app kan få adgang til data i Microsoft Graph, skal brugeren eller administratoren give den de rette tilladelser via en samtykkeproces. [Reference til Microsoft Graph-tilladelser](https://docs.microsoft.com/graph/permissions-reference) viser de tilladelser, der er knyttet til hvert overordnede sæt Microsoft Graph-API'er. Den indeholder også en vejledning til, hvordan du bruger tilladelserne.

**Konfigurer eller opdater tjenesteinspektør**

- [Opret serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) – I denne artikel kan du se, hvordan du opretter et nyt servicePrincipal-objekt.
- [Opret en Azure AD-app](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) &-tjenesteinspektør på portalen – Denne artikel viser, hvordan du opretter et nyt Azure Active Directory-program (Azure AD) og en tjenesteinspektør, der kan bruges sammen med det rollebaserede adgangskontrolelement.
- [Apps & tjenesteinspektører](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) i Azure AD – I denne artikel beskrives programregistrering, programobjekter og tjeneste principaler i Azure Active Directory: hvad de er, hvordan de bruges, og hvordan de er relateret til hinanden.

**Tilføj eller opdater appregistrering, og giv administratorsamtykke**

- [Opret en appregistrering –](https://docs.microsoft.com/graph/api/application-post-applications) I denne artikel kan du se, hvordan du opretter et nyt programobjekt.
- [Opdater en appregistrering – API-tilladelser](https://docs.microsoft.com/graph/api/application-update) – Denne artikel viser, hvordan du opdaterer egenskaberne for et programobjekt.
- [Giv administratorsamtykke](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) – For at give administratorsamtykke og samtykke generelt kræver vi, at en administrator udtrykkeligt giver samtykke.
- [RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) – Rollestyringsbeholder til samlede rolledefinitioner og rolletildelinger til Microsoft 365 RBAC-udbydere, der understøtter flere hovedstole og flere områder i en enkelt rolletildeling. Dette er forskelligt *fra ressourcetypen rbacApplication.* Microsoft Intune er et eksempel på en sådan RBAC-udbyder. En rolletildeling i Intune kan have en række hovedstole og en række omfangsgrupper. **Dette er i beta, hvilket betyder, at den stadig er under udvikling og ikke anbefales til brug i produktion.**
