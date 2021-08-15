---
title: Problemer med udvikling af programmer med API'er
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
- "7755"
ms.openlocfilehash: 1de4e9aa5078507eecdbe53366e446e733029ecb1342f20ca701fa7f95a06fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013454"
---
# <a name="issues-developing-applications-with-apis"></a>Problemer med udvikling af programmer med API'er

For at begynde at bruge Azure Active Directory Graph API skal du se Startvejledningen til [Azure AD Graph API](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) eller se den interaktive [referencedokumentation](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)til Azure AD Graph API.

**Ophør af support til Azure Active Directory Authentication Library (ADAL) og Azure AD Graph API (AAD Graph)**

**Fra og med d. 30. juni 2020** føjer vi ikke længere nye funktioner til ADAL og Azure AD Graph. Vi yder fortsat teknisk support og sikkerhedsopdateringer, men vil ikke længere levere funktionsopdateringer.

**Fra og med den 30. juni 2022** stopper vi understøttelsen af ADAL og Azure AD Graph og yder ikke længere teknisk support eller sikkerhedsopdateringer.

Apps, der bruger ADAL på eksisterende os-versioner, fungerer fortsat efter dette tidspunkt, men får ingen teknisk support eller sikkerhedsopdateringer.

Apps, der bruger Azure AD Graph efter dette tidspunkt, modtager muligvis ikke længere svar fra Azure AD Graph slutpunkt.

**ADAL-overførsel**

Vi anbefaler, at du opdaterer [MSAL (Microsoft Authentication Library)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), som har de nyeste funktioner og sikkerhedsopdateringer.

Hvis du bruger Microsoft-apps, skal du vide, at Microsoft er i gang med at overføre sine programmer til MSAL inden slutdatoen for support, hvilket sikrer, at de får glæde af MSALs løbende sikkerheds- og funktionsforbedringer.

1. [Læs ofte stillede spørgsmål om ADAL.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. [Få mere at vide om, hvordan du overfører apps på pr. platform.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. Hvis du har brug for hjælp til at forstå, hvilke af dine apps der bruger ADAL, anbefaler vi, at du gennemgår alle dine apps kildekode og, hvis det er relevant, kontakt eventuelle internetudbydere eller appudbydere. Microsoft-support kan også give dig en liste over alle ikke-Microsoft ADAL-apps i din lejer.

**AAD Graph Migration**

For programmer, der bruger Azure AD Graph, skal du følge vores vejledning til at overføre [Azure AD Graph-apps til Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)

1. [Vores tjekliste til migrering indeholder et startpunkt](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. Din registreringsportal til Azure-app viser, hvilke programmer der bruger AAD Graph. Vi anbefaler, at du gennemser kildekoden til alle dine apps og, hvis det er relevant, skal du kontakte alle internetudbydere eller appudbydere. Microsoft Support kan også give dig en liste over alle AAD-Graph brug i din lejer.
1. Hvis din app skal have adgang til data i Microsoft Graph, skal brugeren eller administratoren give den de rette tilladelser via en samtykkeproces. Reference [til Microsoft Graph-tilladelser viser](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) de tilladelser, der er knyttet til hvert overordnede sæt af Microsoft-Graph API'er. Den indeholder også vejledning til, hvordan du bruger tilladelserne.
