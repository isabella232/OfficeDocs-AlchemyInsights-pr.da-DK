---
title: Godkendelsesproblemer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7748"
- "9004339"
ms.openlocfilehash: 53bd0d8f8edaead519d0282239d3a6d338b297b9
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974312"
---
# <a name="authentication-issues"></a>Godkendelsesproblemer

**Leder du efter oplysninger om de AADSTS-fejlkoder, der returneres fra Azure Active Directory (Azure AD) sikkerhedstokentjenesten (STS)?** Se [Azure ad-godkendelse og godkendelsesfejl koder](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) for at finde AADSTS-fejlbeskrivelser, løsninger og nogle forslag til løsninger.

Godkendelsesfejl kan skyldes flere forskellige problemer, hvoraf de fleste genererer en 401-eller 403-fejl. Følgende problemer kan for eksempel alle føre til godkendelsesfejl:

- Ukorrekte [erhvervelses flow](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) for adgangstoken 
- Dårligt konfigurerede [omfang af tilladelser](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 
- Manglende [tilladelse](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

Hvis du vil løse almindelige godkendelsesfejl, skal du prøve nedenstående trin, der passer bedst til den fejl, du modtager. Der kan være flere trin, der gælder for en fejl, du modtager.

- **401 uautoriseret fejl: er dit token gyldigt?**

Kontrollér, at din app præsenterer et gyldigt adgangstoken til Microsoft Graph som en del af anmodningen. Denne fejl betyder ofte, at der muligvis mangler et adgangstoken i HTTP-godkendelses anmodningens overskrift, eller at tokenet er ugyldigt eller udløbet. Vi anbefaler på det kraftigste, at du bruger Microsoft-godkendelses bibliotek (MSAL) til hentning af adgangstoken. Denne fejl kan også opstå, hvis du forsøger at bruge en uddelegeret adgangstoken til en personlig Microsoft-konto for at få adgang til et API, der kun understøtter arbejds-eller skole konti (virksomhedskonti).

**403 forbudt fejl: har du valgt det rigtige sæt af tilladelser?**

Kontrollér, at du har anmodet om det korrekte sæt tilladelser på baggrund af Microsoft Graph-API'erne til dine app-opkald. Der findes anbefalede tilladelser til færrest rettigheder i alle emner i Microsoft Graph API-referencemetoden. Desuden skal disse tilladelser tildeles til ansøgningen af en bruger eller en administrator. Tildeling af tilladelser normalt sker gennem en tilladelses side eller brugen af registrerings bladet Azure-Portal program. Fra bladet **Indstillinger** for programmet skal du klikke på **nødvendige tilladelser** og derefter klikke på **Giv tilladelser**. Du kan finde flere oplysninger under:

- [Microsoft Graph-tilladelser](https://docs.microsoft.com/graph/permissions-reference) 
- [Om Azure AD-tilladelser og-samtykke](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**403 forbudt fejl: fik appen fat i et token, så det stemmer overens med de valgte tilladelser?**

Sørg for, at de typer af tilladelser, der anmodes om eller tildeles, passer til den type adgangstoken, din app får. Du anmoder muligvis om og tildeler app-tilladelser, men bruger delegeret interaktiv kode-tokens i stedet for flow-tokens til klientlegitimationsoplysninger eller anmodning om og tildeling af delegerede tilladelser, men brug af tokens til flow af klientlegitimationsoplysninger i stedet for delegeret kode flow-tokens.

Du kan finde flere oplysninger om erhvervende tokens i:

- [Få adgang på vegne af brugere og delegeret tilladelser](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v 2.0-OAuth 2,0 Authorization Code flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Få adgang uden en bruger (daemon-tjeneste) og program tilladelser](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v 2.0-OAuth 2,0-klientoplysninger flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**403 forbudt fejl: nulstilling af adgangskode**

Der er i øjeblikket ingen program rettigheds-daemon-tjenestetilladelser, der tillader nulstilling af brugeradgangskoder. Disse API'er understøttes kun ved hjælp af den interaktive Delegate-kode, der er logget på med en administrator. Du kan finde flere oplysninger i [Microsoft Graph-tilladelser](https://docs.microsoft.com/graph/permissions-reference).

**403 forbudt: har brugeren adgang, og er de givet i licens?**

For delegeret kode-flow evaluerer Microsoft Graph, om anmodningen er blevet tilladt ud fra de tilladelser, der er tildelt til appen, og de tilladelser, som den bruger, der er logget på. Denne fejl tyder normalt på, at brugeren ikke er privilegeret nok til at udføre anmodningen, **eller** at brugeren ikke har licens til at få adgang til dataene. Det er kun brugere med de påkrævede tilladelser eller licenser, der kan udføre anmodningen.

**403 forbudt: har du valgt den korrekte ressource-API?**

API-tjenester som Microsoft Graph Kontrollér, at *AUD* -kravet (publikum) i det modtagne adgangstoken stemmer overens med den værdi, det forventer for sig selv, og hvis det ikke er tilfældet, opstår der en 403 forbudt-fejl. En almindelig fejl, der medfører, at denne fejl forsøger at bruge et token, der er erhvervet til Azure AD Graph-API'er, Outlook-API'er eller SharePoint/OneDrive-API'er til at ringe til Microsoft Graph (eller omvendt). Kontrollér, at den ressource (eller omfanget), som din app henter et token for, passer til API'ET, som appen ringer til.

**400 forkert anmodning eller 403 forbudt: bruger brugeren deres organisations politikker for betinget adgang (CAS)?**

Baseret på en organisations politikker for betinget adgang (CAS) er en bruger, der har adgang til Microsoft Graph-ressourcer via din app, muligvis en udfordring for flere oplysninger, der ikke findes i den adgangstoken, din app oprindeligt har erhvervet. I dette tilfælde modtager din app en **400 med en *interaction_required*** fejl i forbindelse med erhvervelse af adgangstoken eller en **403 med *insufficient_claims*** fejl, når du ringer til Microsoft Graph. I begge tilfælde indeholder fejl svaret flere oplysninger, der kan præsenteres for det godkendte slutpunkt for at udfordre brugeren til yderligere oplysninger (som f. eks. multifaktorgodkendelse eller enheds tilmelding).

Hvis du vil have mere at vide om betinget adgang, skal du se:

- [Håndtering af betingede adgangs udfordringer ved hjælp af MSAL](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Udvikler vejledning til betinget adgang til Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

**_Slutningen af understøttelse af Azure Active Directory-godkendelses bibliotek (ADAL) og Azure ad Graph API (Aad-graf)_* _

- Fra juni 30th, 2020, vil vi ikke længere tilføje nye funktioner til Azure Active Directory-godkendelses bibliotek (ADAL) og Azure AD graf API (AAD-graf). Vi vil fortsat yde teknisk support og sikkerhedsopdateringer, men vil ikke længere tilbyde FUNKTIONSOPDATERINGER.
- Fra juni 30th, 2022, vi afslutter support til ADAL og AAD-grafen og vil ikke længere yde teknisk support eller sikkerhedsopdateringer.
    - Apps, der bruger ADAL på eksisterende OS-versioner, vil fortsat fungere efter dette tidspunkt, men de får ikke teknisk support eller sikkerhedsopdateringer.
    - Apps, der bruger AAD Graph efter dette tidspunkt, kan muligvis ikke længere modtage svar fra AAD-diagram slutpunktet.

_ *ADAL-overførsel**

Vi anbefaler, at du opdaterer til [Microsoft-godkendelses bibliotek (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), som har de nyeste funktioner og sikkerhedsopdateringer. Denne anbefaling er i forbindelse med Microsoft overførsel af sine programmer til MSAL ved hjælp af deadline for ophør. Målsætningen for Microsoft-apps overføres til MSAL er at sikre, at de pågældende apps drager fordel af MSALs fortsatte sikkerheds-og funktionsforbedringer.

- [Læs ADAL ofte stillede spørgsmål](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Få mere at vide om, hvordan du kan overføre apps på et enkelt platforms grundlag](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Hvis du har brug for hjælp til at forstå, hvilke af dine apps der bruger ADAL, anbefaler vi, at du gennemgår alle dine apps-kildekode, og hvis det er relevant, kan du få adgang til alle uafhængige softwareleverandører eller app-udbydere. Microsoft Support kan også give dig en liste over alle ikke-Microsoft-ADAL-apps i din lejer.

**AAD-diagram overførsel**

For programmer, der bruger AAD-graf, skal du følge vores vejledning til at [overføre Azure ad Graph-apps til Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [Vores overflytnings checkliste giver et](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)introduktions point. 
- Din Azure-app-registrerings Portal viser, hvilke programmer der bruger AAD-grafer. Vi anbefaler, at du gennemgår alle din apps-kildekode, og hvis det er relevant, så du kan få adgang til alle ISV'er-eller app-udbydere. Microsoft Support kan også give dig oplysninger om alle AAD-diagram brug i din lejer.

 










