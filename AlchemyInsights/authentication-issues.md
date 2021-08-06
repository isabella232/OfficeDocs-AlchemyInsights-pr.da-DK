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
ms.openlocfilehash: c7e6d96940f8d7052ee4b49b22c0d1d7d5bd5f9277f4a7eff709def1da2e13af
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019502"
---
# <a name="authentication-issues"></a>Godkendelsesproblemer

**Leder du efter oplysninger om AADSTS-fejlkoder, der returneres fra Azure AD (Azure Active Directory) sikkerhedstokentjenesten (STS)?** Se [Azure AD-godkendelses- og autorisationsfejlkoder](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) for at finde AADSTS-fejlbeskrivelser, rettelser og nogle foreslåede midlertidige løsninger.

Autorisationsfejl kan være et resultat af flere forskellige problemer, hvoraf de fleste genererer en 401- eller 403-fejl. F.eks. kan følgende problemer alle føre til autorisationsfejl:

- Forkerte [flows for erhvervelse af adgangstoken](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) 
- Dårligt konfigurerede [rettighedsområder](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 
- Manglende [samtykke](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

For at løse almindelige autorisationsfejl kan du prøve de trin, der er angivet nedenfor, og som passer bedst til den fejl, du modtager. Der kan gælde mere end ét trin for en fejl, du modtager.

**401 Uautoriseret fejl: Er dit token gyldigt?**

Kontrollér, at din app præsenterer et gyldigt adgangstoken til Microsoft Graph som en del af anmodningen. Denne fejl betyder ofte, at adgangstokenet mangler i HTTP-godkendelsesanmodningens header, eller at tokenet er ugyldigt eller er udløbet. Vi anbefaler på det kraftigste, at du bruger MSAL (Microsoft Authentication Library) til erhvervelse af adgangstoken. Desuden kan denne fejl opstå, hvis du forsøger at bruge et delegeret adgangstoken tildelt en personlig Microsoft-konto til at få adgang til en API, der kun understøtter arbejds- eller skolekonti (organisationskonti).

**403 Forbudt fejl: Har du valgt det korrekte sæt af tilladelser?**

Sørg for, at du har anmodet om det korrekte sæt tilladelser baseret på Microsoft Graph-API'er til dine app-opkald. Anbefalet at der gives færrest mulige rettigheder som vist i alle emner om Microsoft Graph API-referencemetode. Desuden skal disse tilladelser til programmet, tildeles af en bruger eller en administrator. Tildeling af tilladelser sker normalt via en samtykkeside eller brug af Azure Portal-programregistreringsbladet. Fra programmets **Indstillinger**-blad, skal du klikke på **Krævede tilladelser**, og derefter klikke på **Giv tilladelser**. Du kan finde flere oplysninger under:

- [Microsoft Graph-tilladelser](https://docs.microsoft.com/graph/permissions-reference) 
- [Om azure AD-tilladelser og -samtykke](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**403 Forbudt fejl: Modtog din app et token, svarende til de valgte tilladelser?**

Sørg for, at de tilladelsestyper, der anmodes om eller tildeles, svarer til adgangstokentypen, som din app modtager. Du anmoder måske om og tildeler apptilladelser, men bruger delegerede interaktive kodeflowtokens i stedet for klientlegitimationstokens, eller anmoder om og tildeler delegerede tilladelser, men bruger klientlegitimationsoplysninger til flowtokens i stedet for delegerede kodeflowtokens.

Du kan finde flere oplysninger om at modtage tokens i:

- [Få adgang på vegne af brugere og delegerede tilladelser](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v2.0 – OAuth 2.0-godkendelseskodeflow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Få adgang uden en bruger (daemon-tjeneste) og programtilladelser](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v2.0 – OAuth 2.0 flow af legitimationsoplysninger](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**403 Forbudt fejl: Nulstilling af adgangskode**

Der er i øjeblikket ingen programtilladelses-daemon-tjeneste-til-tjeneste-tilladelser, der tillader nulstilling af brugeradgangskoder. Disse API'er understøttes kun ved hjælp af de interaktive delegerede kodeflows med en administrator, der er logget på. Få mere at vide under [Microsoft Graph-tilladelser](https://docs.microsoft.com/graph/permissions-reference).

**403 Forbudt: Har brugeren adgang, og har de licens?**

For delegerede kodeflows evaluerer Microsoft Graph, om anmodningen er blevet tilladt, på baggrund af de tilladelser, der er tildelt appen, og de tilladelser, som brugeren, der er logget på, har. Generelt indikerer denne fejl, at brugeren ikke har rettigheder nok til at udføre anmodningen **eller** at brugeren ikke har licens til de data, der fås adgang til. Kun brugere med de nødvendige tilladelser eller licenser kan foretage anmodningen.

**403 Forbudt: Har du valgt den korrekte ressource-API?**

API-tjenester som f.eks. Microsoft Graph kontrollerer, at *aud*-krav (målgruppe) i den modtagne adgangstoken svarer til den værdi, den forventer for sig selv, og hvis ikke, opstår der en 403 Forbudt fejl. En almindelig fejl, der medfører denne fejl, er at forsøge at bruge en token, der er mortaget til Azure AD Graph APIs, Outlook APIs eller SharePoint/OneDrive APIs til at kalde Microsoft Graph (eller omvendt). Sørg for, at ressourcen (eller omfanget) din app henter et token for svarer til den API, som appen kalder.

**400 Forkert anmodning eller 403 Forbudt: Overholder brugeren organisationens politikker for betinget adgang (Conditional Access – CA) ?**

Baseret på en organisations politikker for betinget adgang (CA) kan en bruger, der tilgår Microsoft Graph-ressourcer via din app, blive udfordret med yderligere oplysninger, der ikke findes i den adgangstoken, din app oprindeligt modtog. I dette tilfælde modtager din app en **400 med en *interaction_required***-fejl under modtagelsen af adgangstoken **403 med *insufficient_claims***-fejl, når du kalder Microsoft Graph. I begge tilfælde indeholder fejlsvaret yderligere oplysninger, der kan præsenteres for det autoriserede slutpunkt til at udfordre brugeren for at få yderligere oplysninger (f.eks. multifaktorgodkendelse eller enhedsregistrering).

Du kan finde flere oplysninger om betinget adgang under:

- [Håndtering af betinget adgang-udfordringer ved hjælp af MSAL](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Vejledning for udviklere om Azure Active Directory-betinget adgang](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

***Ophør af support til Azure Active Directory Authentication Library (ADAL) og Azure AD Graph API (AAD Graph)***

- Fra d. 30. juni 2020 tilføjer vi ikke længere nye funktioner til ADAL (Azure Active Directory Authentication Library) og AAD Graph (Azure AD Graph API). Vi yder fortsat teknisk support og sikkerhedsopdateringer, men vil ikke længere levere funktionsopdateringer.
- Fra d. 30. juni 2022 afslutter vi supporten af ADAL og AAD Graph og yder ikke længere teknisk support eller sikkerhedsopdateringer.
    - Apps, der bruger ADAL på eksisterende os-versioner, fungerer fortsat efter dette tidspunkt, men får ingen teknisk support eller sikkerhedsopdateringer.
    - Apps, der bruger AAD Graph efter dette tidspunkt, modtager muligvis ikke længere svar fra AAD Graph-slutpunktet.

**ADAL-overførsel**

Vi anbefaler, at du opdaterer [MSAL (Microsoft Authentication Library)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), som har de nyeste funktioner og sikkerhedsopdateringer. Denne anbefaling er i forbindelse med Microsofts migrering af deres programmer til MSAL ved deadline for slutdato for support. Formålet med Microsoft-apps migrering til MSAL er at sikre, at appsene drage fordel af MSAL's løbende forbedringer af sikkerhed og funktioner.

- [Læs ofte stillede spørgsmål om ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Få mere at vide om at migrere apps pr. platform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Hvis du har brug for hjælp til at forstå, hvilke af dine apps der bruger ADAL, anbefaler vi, at du gennemser alle dine apps' kildekode, og hvis det er relevant, skal du kontakte eventuelle ISV'er (uafhængige softwareleverandører) eller appudbydere. Microsoft-support kan også give dig en liste over alle ikke-Microsoft ADAL-apps i din lejer.

**AAD Graph Migration**

For programmer, der bruger AAD Graph, skal du følge vores vejledning i at [migrere Azure AD Graph-apps til Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [Vores tjekliste til migrering indeholder et startpunkt](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- Din registreringsportal til Azure-app viser, hvilke programmer der bruger AAD Graph. Vi anbefaler, at du gennemser kildekoden til alle dine apps og, hvis det er relevant, skal du kontakte alle internetudbydere eller appudbydere. Microsoft Support kan også give dig oplysninger om brug al AAD Graph-i din lejer.

 










