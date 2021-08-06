---
title: Forespørgsel i Microsoft Graph API
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
ms.openlocfilehash: eda5d8d1d76d0d87312b1441aeae89d8e250abe0e8b613d4a43fcc2345a6f021
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923233"
---
# <a name="querying-the-microsoft-graph-api"></a>Forespørgsel i Microsoft Graph API

Dette emne kan også gælde for udviklere, der stadig bruger Azure AD Graph API. Det anbefales dog på **det kraftigste,** at du bruger Microsoft Graph til alle scenarierne katalog, identitet og adgangsstyring.

**Godkendelses- eller godkendelsesproblemer**

- Hvis din app ikke kan købe **tokens** til at kalde Microsoft Graph, skal du vælge Problem med at få en adgangstoken **(godkendelse)** kategori for Microsoft Graph for at få mere specifik hjælp og support til dette emne.
- Hvis din app modtager **401-** eller 403-godkendelsesfejl, når du kalder Microsoft Graph, skal du vælge kategorien Får en adgang nægtet fejl **(godkendelse)** Microsoft Graph API for at få mere specifik hjælp og support til dette emne.

**Jeg vil bruge Microsoft Graph, men jeg er ikke sikker på, hvor jeg skal starte**

Du kan få mere at vide om Microsoft Graph i:

- [Oversigt over Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Oversigt over identitets- og adgangsstyring i Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Kom i gang med at bygge Microsoft Graph-apps](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – Test Microsoft Graph-API'er i din lejer eller en demolejer

**Jeg vil bruge Microsoft Graph, men understøtter det de v1.0-mappe-API'er, jeg har brug for?**

Microsoft Graph er den anbefalede API til administration af kataloger, identitet og adgang. Der er dog stadig nogle få mellemrum mellem, hvad der er muligt i Azure AD Graph og Microsoft Graph. Gennemgå følgende artikler, som fremhæver de mest opdaterede forskelle, der kan hjælpe dig med dit valg:

- [Forskelle mellem ressourcetyper mellem Azure AD Graph og Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Egenskabsforskelle mellem Azure AD Graph og Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Forskelle mellem Azure AD og Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Når jeg *forespørger* i brugerobjektet, mangler mange af dets egenskaber**

`GET https://graph.microsoft.com/v1.0/users` returnerer kun 11 egenskaber, da Microsoft Graph automatisk vælger et standardsæt af *brugeregenskaber, der* skal returneres. Hvis du har brug for *andre brugeregenskaber,* kan $select til at vælge de egenskaber, programmet skal bruge. Prøv det i **Microsoft Graph Explorer** først.

**Nogle brugeregenskabsværdier er *null,* selvom jeg ved, at de er angivet**

Den mest sandsynlige forklaring er, at programmet har fået *tilladelsen User.ReadBasic.All.* Dette giver programmet mulighed for at læse et begrænset sæt af brugeregenskaber og returnere alle andre egenskaber som null, selvom de tidligere er blevet angivet. Prøv i stedet at tildele *programmet User.Read.All-tilladelse.*

Du kan få mere at vide [under Brugertilladelser i Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference#user-permissions).

**Jeg har problemer med at bruge OData-forespørgselsparametre til at filtrere data i mine anmodninger**

Selvom Microsoft Graph understøtter en lang række OData-forespørgselsparametre, understøttes mange af disse parametre ikke fuldt ud af katalogtjenester (ressourcer, der nedarver fra *directoryObject)* i Microsoft Graph. De samme begrænsninger, der var til stede i Azure AD Graph, bevares for det meste i Microsoft Graph:

1. **Ikke understøttet:**$count, $search og $filter ved *null-* *eller ikke Null-værdier*
2. **Ikke understøttet:**$filter på bestemte egenskaber (se ressourceemner, hvor egenskaberne kan filtreres)
3. **Ikke understøttet:** sideinddeling, filtrering og sortering på samme tid
4. **Ikke understøttet:** filtrering af en relation. For eksempel – find alle medlemmer af den tekniske gruppe, der befinder sig i Storbritannien.
5. **Delvis understøttelse:**$orderby *på bruger* (kun displayName og userPrincipalName) og *gruppe*
6. **Delvis understøttelse:**$filter (understøtter kun *lige*,  *starter* med *,* eller og , og har begrænset nogen *)* understøttelse, returnerer $expand (når et enkelt objekts relationer udvides, returneres alle relationer, men det er begrænset, at en samling af objekters relationer udvides)

Få mere at vide under [Tilpas svar med forespørgselsparametre.](https://docs.microsoft.com/graph/query-parameters)

**Den API, jeg ringer til, virker ikke – hvor kan jeg udføre flere test?**

**Microsoft Graph Explorer** – Test Microsoft Graph-API'er i din lejer eller en demolejer, og se også **eksempelforespørgsler** i Microsoft Graph Explorer.

**Når jeg forespørger efter data, ser det ud til, at jeg får et ufuldstændigt datasæt tilbage**

Hvis du forespørger på en samling (f.eks. *brugere),* bruger Microsoft Graph begrænsninger på serversiden, så resultaterne returneres altid med en standardsidestørrelse. Din app bør altid forvente at side gennem samlinger, der returneres fra tjenesten.

Du kan finde flere oplysninger under:

- [Bedste fremgangsmåder for Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Sideinddeling af Microsoft Graph-data i din app](https://docs.microsoft.com/graph/paging)

**Min app er for langsom og bliver også begrænser. Hvilke forbedringer kan jeg foretage?**

Afhængigt af scenariet er der en række forskellige muligheder til din rådighed for at gøre programmet mere performant og i nogle tilfælde mindre tilbøjelig til at blive begrænser af tjenesten (når du foretager for mange opkald).

Du kan få mere at vide under:

- [Bedste fremgangsmåder for Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Batching af anmodninger](https://docs.microsoft.com/graph/json-batching)
- [Registrere ændringer via deltaforespørgsel](https://docs.microsoft.com/graph/delta-query-overview)
- [Få besked om ændringer via webhooks](https://docs.microsoft.com/graph/webhooks)
- [Begrænsningsvejledning](https://docs.microsoft.com/graph/throttling)

**Hvor kan jeg finde flere oplysninger om fejl og kendte problemer?**

- [Oplysninger om fejlsvar i Microsoft Graph](https://docs.microsoft.com/graph/errors)
- [Kendte problemer med Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Hvor kan jeg kontrollere status for tjenestens tilgængelighed og forbindelse?**

Tjenestens tilgængelighed og forbindelse mellem de underliggende tjenester, der kan tilgås via Microsoft Graph, kan påvirke den samlede tilgængelighed og ydeevne i Microsoft Graph.

- For Azure Active Directory-tjenestetilstand skal du kontrollere status for **Sikkerhed + identitetstjenester,** der er angivet på [siden Azure-status.](https://azure.microsoft.com/status/)
- For Office-tjenester, der bidrager til Microsoft Graph, skal du kontrollere status for tjenester, der er angivet i [Dashboard for tjenestetilstand i Office.](https://portal.office.com/adminportal/home#/servicehealth)
