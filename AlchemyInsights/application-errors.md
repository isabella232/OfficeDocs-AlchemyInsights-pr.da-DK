---
title: Programfejl
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
- "9004342"
- "7841"
ms.openlocfilehash: 2ef90b54ce222a06740e05891fabe87b6565cb14
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/25/2021
ms.locfileid: "49984542"
---
# <a name="application-errors"></a>Programfejl

Leder du efter oplysninger om de **AADSTS-fejlkoder** , der returneres fra Azure Active Directory (Azure ad)-SIKKERHEDSTOKENTJENESTEN (STS)? Læs [Azure ad-godkendelse og godkendelsesfejl koder](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) for at finde AADSTS-fejlbeskrivelser, løsninger og nogle forslag til løsninger.

Godkendelsesfejl kan skyldes flere forskellige problemer, hvoraf de fleste genererer en 401-eller 403-fejl. For eksempel kan det være, at følgende kan føre til godkendelsesfejl:

- Ukorrekte [erhvervelses flow](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) for adgangstoken 
- Dårligt konfigurerede [omfang af tilladelser](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- Manglende [tilladelse](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

Hvis du vil løse almindelige godkendelsesfejl, skal du prøve nedenstående trin, der passer bedst til den fejl, du modtager. Der kan blive anvendt mere end én.

**401 uautoriseret fejl: er dit token gyldigt?**

Sørg for, at dit program præsenterer et gyldigt adgangstoken til Microsoft Graph som en del af anmodningen. Denne fejl betyder ofte, at der muligvis mangler et adgangstoken i HTTP-godkendelses anmodningens overskrift, eller at tokenet er ugyldigt eller udløbet. Vi anbefaler på det kraftigste, at du bruger [Microsoft-godkendelses bibliotek (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) til hentning af adgangstoken. Denne fejl kan også opstå, hvis du forsøger at bruge en uddelegeret adgangstoken til en personlig Microsoft-konto for at få adgang til et API, der kun understøtter arbejds-eller skole konti (organisations konti).

**403 forbudt fejl: har du valgt det rigtige sæt af tilladelser?**

Kontrollér, at du har anmodet om det korrekte sæt af tilladelser, der er baseret på Microsoft Graph-API'erne til dine app-opkald. Anbefalede minimum rettigheder er angivet i alle emner i Microsoft Graph API-referencemetoden. Desuden skal disse tilladelser tildeles til ansøgningen af en bruger eller en administrator. Tildeling af tilladelser normalt sker gennem en tilladelses side eller ved at tildele tilladelser ved hjælp af registrerings bladet Azure Portal-program. Fra bladet **Indstillinger** for programmet skal du klikke på **nødvendige tilladelser** og derefter klikke på **Giv tilladelser**.

- [Microsoft Graph-tilladelser](https://docs.microsoft.com/graph/permissions-reference) 
- [Om Azure AD-tilladelser og-samtykke](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**403 forbudt fejl: fik appen fat i et token, så det stemmer overens med de valgte tilladelser?**

Sørg for, at den type af tilladelser, der anmodes om eller tildeles, passer til den type adgangstoken, din app henter. Du anmoder muligvis om og tildeler program tilladelser, men bruger delegeret interaktiv kode-tokens i stedet for flow-tokens til klientlegitimationsoplysninger eller anmodning om og tildeling af stedfortrædertilladelser, men brug af tokens til flow af klientlegitimationsoplysninger i stedet for delegeret kode flow-tokens.

- [Få adgang på vegne af brugere og delegeret tilladelser](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v 2.0-OAuth 2,0 Authorization Code flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Få adgang uden en bruger (daemon-tjeneste) og program tilladelser](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v 2.0-OAuth 2,0-klientoplysninger flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**403 forbudt fejl: nulstilling af adgangskode**

Der er i øjeblikket ingen program rettigheds-daemon-tjenestetilladelser, der tillader nulstilling af brugeradgangskoder. Disse API'er understøttes kun ved hjælp af den interaktive Delegate-kode, der er logget på med en administrator.

- [Microsoft Graph-tilladelser](https://docs.microsoft.com/graph/permissions-reference)

**403 forbudt: har brugeren adgang, og er de givet i licens?**

For delegeret kode strømme evaluerer Microsoft Graph, om anmodningen er tilladt baseret på de tilladelser, der er tildelt appen, og de tilladelser, som den bruger, der er logget på. Denne fejl tyder normalt på, at brugeren ikke er privilegeret nok til at udføre anmodningen, eller at brugeren ikke har licens til at få adgang til dataene. Det er kun brugere med de påkrævede tilladelser eller licenser, der kan udføre anmodningen.

**403 forbudt: har du valgt den korrekte ressource-API?**

API-tjenester som Microsoft Graph Kontrollér, at AUD-kravet (publikum) i det modtagne adgangstoken stemmer overens med den værdi, det forventer for sig selv, og hvis ikke, det resulterer i en 403-forbudt fejl. En almindelig fejl, der medfører, at denne fejl forsøger at bruge et token, der er erhvervet til Azure AD Graph-API'er, Outlook-API'er eller SharePoint/OneDrive-API'er til at ringe til Microsoft Graph (eller omvendt). Kontrollér, at den ressource (eller omfanget), som din app henter et token for, passer til API'ET, som appen ringer til.

**400 forkert anmodning eller 403 forbudt: bruger brugeren deres organisations politikker for betinget adgang (CAS)?**

Baseret på en organisations CAS-politikker, kan en bruger, der har adgang til Microsoft Graph-ressourcer via din app, blive udfordringt om yderligere oplysninger, der ikke findes i den adgangstoken, din app oprindeligt har erhvervet. I dette tilfælde modtager din app en 400 med en *interaction_required* fejl i forbindelse med erhvervelse af adgangstoken eller en 403 med *insufficient_claims* fejl, når du ringer til Microsoft Graph. I begge tilfælde indeholder fejl svaret flere oplysninger, der kan præsenteres for godkendelses slutpunktet for at give brugeren yderligere oplysninger (som f. eks. multifaktorgodkendelse eller enheds tilmelding).

- [Håndtering af betingede adgangs udfordringer ved hjælp af MSAL ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Udvikler vejledning til betinget adgang til Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
