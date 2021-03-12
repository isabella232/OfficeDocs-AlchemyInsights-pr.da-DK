---
title: Problemer med Microsoft Graph API
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
- "9004345"
- "7759"
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/29/2021
ms.locfileid: "50713471"
---
# <a name="microsoft-graph-api-issues"></a>Problemer med Microsoft Graph API

Dette emne kan også gælde for udviklere, der stadig bruger Azure AD Graph API. Det anbefales dog på **det kraftigste,** at du bruger Microsoft Graph til alle scenarierne administration af katalog, identitet og adgang.

**Godkendelses- eller godkendelsesproblemer**

- Hvis din app ikke kan få **tokens** til at kalde Microsoft Graph, skal du vælge Problem med at få en adgangstoken **(godkendelse)** kategori for Microsoft Graph for at få mere specifik hjælp og support til dette emne.
- Hvis din app modtager **401-** eller 403-godkendelsesfejl, når du kalder Microsoft Graph, skal du vælge kategorien Få en adgang nægtet-fejl **(Godkendelse)** Microsoft Graph API for at få mere specifik hjælp og support i dette emne.

**Jeg vil bruge Microsoft Graph, men jeg er ikke sikker på, hvor jeg skal starte**

- [Oversigt over Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Oversigt over identitets- og adgangsstyring i Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Introduktion til at bygge Microsoft Graph-apps](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – Test Microsoft Graph-API'er i din lejer eller en demolejer

**Jeg vil bruge Microsoft Graph, men understøtter den de v1.0-mappe-API'er, jeg har brug for?**

Microsoft Graph er den anbefalede API til administration af kataloger, identiteter og adgang. Der er dog stadig nogle få mellemrum mellem, hvad der er muligt i Azure AD Graph og Microsoft Graph. Gennemgå følgende artikler, som fremhæver de mest opdaterede forskelle, der kan hjælpe dig med dit valg:

- [Forskelle i ressourcetyper mellem Azure AD Graph og Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Egenskabsforskelle mellem Azure AD Graph og Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Forskelle på metoden mellem Azure AD og Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**API'en, jeg ringer til, fungerer ikke – hvor kan jeg udføre flere test?**

**Microsoft Graph Explorer** – Test Microsoft Graph-API'er i din lejer eller en demolejer, og se også **eksempelforespørgsler** i Microsoft Graph Explorer.

**Min app er for langsom og bliver også begrænser. Hvilke forbedringer kan jeg foretage?**

Afhængigt af scenariet er der en række forskellige muligheder til rådighed for at gøre dit program mere performant, og i nogle tilfælde mindre tilbøjelig til at blive begrænser af tjenesten (når du foretager for mange opkald).

- [Bedste fremgangsmåder for Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Batching af anmodninger](https://docs.microsoft.com/graph/json-batching)
- [Registrer ændringer via deltaforespørgsel](https://docs.microsoft.com/graph/delta-query-overview)
- [Få besked om ændringer via webhooks](https://docs.microsoft.com/graph/webhooks)
- [Begrænsningsvejledning](https://docs.microsoft.com/graph/throttling)

**Hvor kan jeg finde flere oplysninger om fejl og kendte problemer?**

- [Oplysninger om fejlsvar i Microsoft Graph](https://docs.microsoft.com/graph/errors)
- [Kendte problemer med Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Hvor kan jeg kontrollere status for tjenestens tilgængelighed og forbindelse?**

Tjenestens tilgængelighed og forbindelse til de underliggende tjenester, der kan tilgås via Microsoft Graph, kan påvirke den overordnede tilgængelighed og ydeevne i Microsoft Graph.

- For Azure Active Directory-tjenestetilstand skal du kontrollere status for **Sikkerhed + Identity-tjenester,** der er angivet på [Azure-statussiden.](https://azure.microsoft.com/status/)
- For Office-tjenester, der bidrager til Microsoft Graph, skal du kontrollere status for tjenester, der er angivet på [dashboardet for tjenestetilstand i Office.](https://portal.office.com/adminportal/home#/servicehealth)

Godkendelsesfejl i Microsoft Graph kan skyldes flere forskellige problemer, hvoraf de fleste genererer en 401- eller 403-fejl. Følgende kan f.eks. alle føre til godkendelsesfejl:

- Forkerte [flows for erhvervelse af adgangstoken](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- Dårligt konfigurerede [rettighedsområder](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- Manglende [samtykke](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

**_Slutdato for support af ADAL (Azure Active Directory Authentication Library) og AAD Graph (Azure AD Graph API)_* _

_*Fra d. 30. juni 2020** føjer vi ikke længere nye funktioner til ADAL og Azure AD Graph. Vi yder fortsat teknisk support og sikkerhedsopdateringer, men vil ikke længere levere funktionsopdateringer.

**Fra den 30. juni 2022** afslutter vi understøttelsen af ADAL og Azure AD Graph og yder ikke længere teknisk support eller sikkerhedsopdateringer.

Apps, der bruger ADAL på eksisterende OS-versioner, fungerer fortsat efter dette tidspunkt, men får *ikke teknisk support eller sikkerhedsopdateringer.*

Apps, der bruger Azure AD Graph efter dette tidspunkt, modtager muligvis ikke længere svar fra Azure AD Graph-slutpunktet.

**ADAL-overførsel**

Vi anbefaler, at du opdaterer [MSAL (Microsoft Authentication Library)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), som har de nyeste funktioner og sikkerhedsopdateringer.

Hvis du bruger Microsoft-apps, skal du vide, at Microsoft er i gang med at overføre sine programmer til MSAL inden slutdatoen for support, hvilket sikrer, at de får glæde af MSAL's løbende sikkerheds- og funktionsforbedringer.

1. [Læs ofte stillede spørgsmål om ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Få mere at vide om at migrere apps pr. platform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Hvis du har brug for hjælp til at forstå, hvilke af dine apps der bruger ADAL, anbefaler vi, at du gennemgår alle dine apps kildekode og, hvis det er relevant, tager kontakt til eventuelle internetudbydere eller appudbydere. Microsoft-support kan også give dig en liste over alle ikke-Microsoft ADAL-apps i din lejer.

**AAD Graph Migration**

For programmer, der bruger Azure AD Graph, skal du følge vores vejledning til [at overføre Azure AD Graph-apps til Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Vores tjekliste til migrering indeholder et startpunkt](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. Din registreringsportal til Azure-app viser, hvilke programmer der bruger AAD Graph. Vi anbefaler, at du gennemser kildekoden til alle dine apps og, hvis det er relevant, skal du kontakte alle internetudbydere eller appudbydere. Microsoft Support kan også give dig en liste over al AAD Graph-brug i din lejer.
3. Hvis din app skal have adgang til data i Microsoft Graph, skal brugeren eller administratoren give den de rette tilladelser via en samtykkeproces. [Tilladelsesreferencen for Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) viser de tilladelser, der er knyttet til hvert overordnede sæt af Microsoft Graph-API'er. Den indeholder også en vejledning til, hvordan du bruger tilladelserne.
