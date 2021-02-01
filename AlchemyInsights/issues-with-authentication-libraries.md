---
title: Problemer med godkendelsesbiblioteker
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004333"
- "7731"
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063589"
---
# <a name="issues-with-authentication-libraries"></a>Problemer med godkendelsesbiblioteker

1. [Godkendelsesbiblioteker for Microsoft-identitetsplatformen](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) viser microsoft-understøttede og kompatible klient- og middlewarebiblioteker.
2. Microsoft Authentication Library (MSAL) understøtter flere [godkendelsesflows](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) til brug i forskellige programscenarier.
3. For at godkende og anskaffe tokens skal du initialisere et nyt offentligt eller fortroligt klientprogram i din kode. Du kan angive flere konfigurationsindstillinger, når du initialiserer klientappen i Microsoft-godkendelsesbiblioteket (MSAL). Du kan få mere at vide under [Indstillinger for programkonfiguration.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)

**Ophør af understøttelse af Azure Active Directory Authentication Library (ADAL) og Azure AD Graph API (AAD Graph)**

**Fra den 30. juni 2020** tilføjer vi ikke længere nye funktioner til ADAL og Azure AD Graph. Vi yder fortsat teknisk support og sikkerhedsopdateringer, men vil ikke længere levere funktionsopdateringer.

**Fra den 30. juni 2022** afslutter vi understøttelsen af ADAL og Azure AD Graph og yder ikke længere teknisk support eller sikkerhedsopdateringer.

Apps, der bruger ADAL på eksisterende os-versioner, vil fortsat fungere efter dette tidspunkt, men vil *ikke få teknisk support eller sikkerhedsopdateringer.*

Apps, der bruger Azure AD Graph efter dette tidspunkt, modtager muligvis ikke længere svar fra Azure AD Graph-slutpunktet.

**ADAL-overførsel**

Vi anbefaler, at du opdaterer [MSAL (Microsoft Authentication Library)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), som har de nyeste funktioner og sikkerhedsopdateringer.

Hvis du bruger Microsoft-apps, skal du vide, at Microsoft er i gang med at overføre sine programmer til MSAL inden slutdatoen for support, hvilket sikrer, at de får glæde af MSAL's løbende sikkerheds- og funktionsforbedringer.

Du kan finde flere oplysninger under:

1. [Læs ofte stillede spørgsmål om ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Få mere at vide om at migrere apps pr. platform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Hvis du har brug for hjælp til at forstå, hvilke af dine apps der bruger ADAL, anbefaler vi, at du gennemgår alle dine apps kildekode og, hvis det er relevant, tager kontakt til eventuelle internetudbydere eller appudbydere. Microsoft-support kan også give dig en liste over alle ikke-Microsoft ADAL-apps i din lejer.

**AAD Graph Migration**

For programmer, der bruger Azure AD Graph, skal du følge vores vejledning til [at overføre Azure AD Graph-apps til Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Vores tjekliste til overførsel giver et introduktionspunkt.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Din registreringsportal til Azure-app viser, hvilke programmer der bruger AAD Graph. Vi anbefaler, at du gennemser kildekoden til alle dine apps og, hvis det er relevant, skal du kontakte alle internetudbydere eller appudbydere. Microsoft Support kan også give dig en liste over al AAD Graph-brug i din lejer.
3. For at din app kan få adgang til data i Microsoft Graph, skal brugeren eller administratoren give den de rette tilladelser via en samtykkeproces. [Tilladelsesreferencen for Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) viser de tilladelser, der er knyttet til hvert overordnede sæt af Microsoft Graph-API'er. Den indeholder også en vejledning til, hvordan du bruger tilladelserne.
