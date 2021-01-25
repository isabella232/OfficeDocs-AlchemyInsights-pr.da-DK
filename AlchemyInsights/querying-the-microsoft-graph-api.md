---
title: Forespørgsel til Microsoft Graph API
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
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974283"
---
# <a name="querying-the-microsoft-graph-api"></a>Forespørgsel til Microsoft Graph API

Dette emne gælder muligvis også for udviklere, der stadig bruger Azure AD Graph API. Det anbefales dog på det **kraftigste** , at du bruger Microsoft Graph til alle scenarier for katalog, identitet og adgangsstyring.

**Godkendelses-eller godkendelsesproblemer**

- Hvis din app **ikke kan hente tokens** til at ringe til Microsoft Graph, skal du vælge **problem med at få en Access-token (Authentication)** Microsoft Graph-kategori for at få mere specifik hjælp og support til dette emne.
- Hvis din app **modtager 401-eller 403-godkendelsesfejl** , når du ringer til Microsoft Graph, skal du vælge Microsoft Graph-API **-kategorien få adgang nægtet (godkendelse)** til at få mere specifik hjælp og support i dette emne.

**Jeg vil bruge Microsoft Graph, men ikke sikker på, hvor du skal starte**

Du kan få mere at vide om Microsoft Graph i:

- [Oversigt over Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Oversigt over identitets-og adgangsstyring i Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Introduktion til oprettelse af Microsoft Graph-apps](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** -test Microsoft Graph-API'er i din lejer eller en demo lejer

**Jeg vil bruge Microsoft Graph, men det understøtter ikke det v 1.0-katalog-API'er, jeg har brug for?**

Microsoft Graph er den anbefalede API til katalog, identitet og adgangs administration. Der er dog stadig nogle mellemrum mellem det, der er muligt i Azure AD Graph og Microsoft Graph. Gennemgå følgende artikler, som fremhæver de mest opdaterede forskelle for at hjælpe dig med dit valg:

- [Forskelle mellem ressourcetyperne i Azure AD Graph og Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Forskelle mellem egenskaber mellem Azure AD Graph og Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Metode forskelle mellem Azure AD og Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Når jeg opretter en forespørgsel i *bruger* objektet, mangler der mange egenskaber**

`GET https://graph.microsoft.com/v1.0/users` returnerer kun 11-egenskaber, da Microsoft Graph automatisk vælger et standardsæt af *bruger* egenskaber, der skal returneres. Hvis du har brug for andre *bruger* egenskaber, kan du bruge $Select til at vælge de egenskaber, som programmet skal bruge. Prøv det i **Microsoft Graph Explorer** først.

**Nogle bruger egenskabsværdier er *Null* , også selvom jeg ved, at de er angivet**

Den mest sandsynlige forklaring er, at programmet har fået tildelt *brugeren. ReadBasic. alle* tilladelser. Dette gør det muligt for programmet at læse et begrænset sæt af bruger egenskaber, der returnerer alle andre egenskaber som null, selvom de tidligere er angivet. Prøv at tildele program *brugeren. Læs. alle* tilladelser i stedet.

Du kan finde flere oplysninger i [Microsoft Graph-brugertilladelser](https://docs.microsoft.com/graph/permissions-reference#user-permissions).

**Jeg har problemer med at bruge OData-forespørgselsparametre til at filtrere data i mine anmodninger**

Selvom Microsoft Graph understøtter en lang række OData-forespørgselsparametre, understøttes mange af disse parametre ikke fuldt ud af katalogtjenester (ressourcer, der nedarves fra *directoryObject*) i Microsoft Graph. De samme begrænsninger, der blev vist i Azure AD Graph, bevares i Microsoft Graph:

1. **Understøttes ikke**: $count, $search og $filter på *Null* eller *NOT NULL* -værdier
2. **Understøttes ikke**: $filter på visse egenskaber (Se ressource emner, der indeholder de egenskaber, der kan filtreres)
3. **Understøttes ikke**: paging, filtrering og sortering på samme tid
4. **Understøttes ikke**: filtrering af en relation. For eksempel – Find alle medlemmer af gruppen teknikere, der er i Storbritannien.
5. **Delvis support**: $OrderBy *bruger* (kun DisplayName og userPrincipalName) og *gruppe*
6. **Delvis understøttelse**: $filter (understøtter kun *EQ*-, *StartsWith*- *eller* *og begr* ænset *en*) understøttelse, $Expand (udvidelse af relationerne mellem et enkelt objekt returnerer alle relationer, men udvidelse af en samling af objektrelationer er begrænset)

Hvis du vil have mere at vide, skal du se [tilpasse svar med forespørgselsparametre](https://docs.microsoft.com/graph/query-parameters).

**API'EN, jeg ringer til, fungerer ikke – hvor kan jeg foretage flere tests?**

**Microsoft Graph Explorer** -test Microsoft Graph-API'er i din lejer eller en demo lejer, og se også **eksempel forespørgslerne** i Microsoft Graph Explorer.

**Når jeg opretter en forespørgsel efter data, ser det ud til, at jeg får et ufuldstændigt datasæt tilbage**

Hvis du forespørger en samling (som *brugere*), bruger Microsoft Graph serverside begrænsninger, så resultaterne altid returneres med en standardsidestørrelse. Din app bør altid forvente at side gennem samlinger, der returneres fra tjenesten.

Du kan finde flere oplysninger under:

- [Bedste fremgangsmåder for Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Side om at overskrive Microsoft Graph-data i din app](https://docs.microsoft.com/graph/paging)

**Min app er for langsom og får også begrænset det. Hvilke forbedringer kan jeg lave?**

Afhængigt af dit scenarie er der en række forskellige muligheder for din rådighed til at gøre dit programmere drifts nært, og i nogle tilfælde, hvor du kan blive begrænset af tjenesten (når du foretager for mange opkald).

Du kan få mere at vide under:

- [Bedste fremgangsmåder for Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Anmodninger om batch](https://docs.microsoft.com/graph/json-batching)
- [Registrer ændringer via en Delta forespørgsel](https://docs.microsoft.com/graph/delta-query-overview)
- [Få besked om ændringer via webhooks](https://docs.microsoft.com/graph/webhooks)
- [Begrænset vejledning](https://docs.microsoft.com/graph/throttling)

**Hvor kan jeg finde flere oplysninger om fejl og kendte problemer?**

- [Oplysninger om fejlsvar i Microsoft Graph](https://docs.microsoft.com/graph/errors)
- [Kendte problemer med Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Hvor kan jeg kontrollere status for tjenestens tilgængelighed og forbindelse?**

Tjenestens tilgængelighed og forbindelse mellem de underliggende tjenester, der kan åbnes gennem Microsoft Graph, kan påvirke den overordnede tilgængelighed og ydeevne i Microsoft Graph.

- For Azure Active Directory-tjenestetilstand skal du kontrollere status for **sikkerheds + identitets** tjenester, der er angivet på [siden Azure-status](https://azure.microsoft.com/status/).
- For Office-tjenester, der bidrager til Microsoft Graph, skal du kontrollere status for tjenester, der er angivet i [dashboardet til Office-tjenestetilstand](https://portal.office.com/adminportal/home#/servicehealth).
