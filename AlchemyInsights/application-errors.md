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
ms.openlocfilehash: ce4c89da79112726ed4fb25527edc8d082bd37f239595b9eab7279abeeecfd7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931443"
---
# <a name="application-errors"></a>Programfejl

Leder du efter oplysninger om **AADSTS-fejlkoder,** der returneres fra Azure Active Directory (Azure AD) sikkerhedstokentjeneste (STS)? Læs [Fejlkoder til Azure AD-godkendelse](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) og -godkendelse for at finde AADSTS-fejlbeskrivelser, -rettelser og nogle foreslåede løsninger.

Autorisationsfejl kan være et resultat af flere forskellige problemer, hvoraf de fleste genererer en 401- eller 403-fejl. Følgende kan f.eks. alle føre til godkendelsesfejl:

- Forkerte [flows for erhvervelse af adgangstoken](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- Dårligt konfigurerede [rettighedsområder](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- Manglende [samtykke](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

Du kan løse almindelige godkendelsesfejl ved at prøve de trin nedenfor, der passer bedst til den fejl, du modtager. Der kan gælde mere end én.

**401 Uautoriseret fejl: Er dit token gyldigt?**

Sørg for, at dit program præsenterer et gyldigt adgangstoken til Microsoft Graph som en del af anmodningen. Denne fejl betyder ofte, at adgangstokenet mangler i HTTP-godkendelsesanmodningens header, eller at tokenet er ugyldigt eller er udløbet. Vi anbefaler på det kraftigste, at du [bruger Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) til anskaffelse af adgangstoken. Desuden kan denne fejl opstå, hvis du forsøger at bruge en delegeret adgangstoken, der er tildelt en personlig Microsoft-konto, til at få adgang til en API, der kun understøtter arbejds- eller skolekonti (organisationskonti).

**403 Forbudt fejl: Har du valgt det korrekte sæt af tilladelser?**

Kontrollér, at du har anmodet om det korrekte sæt tilladelser baseret på den Microsoft-Graph API'er dine appopkald. Anbefalede mindst privilegerede tilladelser findes i alle emnerne under Microsoft Graph API-referencemetoden. Desuden skal disse tilladelser til programmet, tildeles af en bruger eller en administrator. Tildeling af tilladelser sker normalt via en samtykkeside eller ved at tildele tilladelser ved hjælp af Azure Portal-programregistrerings bladet. Fra programmets **Indstillinger**-blad, skal du klikke på **Krævede tilladelser**, og derefter klikke på **Giv tilladelser**.

- [Microsoft Graph-tilladelser](https://docs.microsoft.com/graph/permissions-reference) 
- [Om azure AD-tilladelser og -samtykke](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**403 Forbudt fejl: Modtog din app et token, svarende til de valgte tilladelser?**

Sørg for, at den type tilladelser, der anmodes om eller tildeles, svarer til den type adgangstoken, som din app får. Du anmoder og giver muligvis programtilladelser, men bruger delegerede interaktive kodeflowtokens i stedet for tokens for flow af klientoplysninger eller anmoder om og tildeler delegerede tilladelser, men bruger klientlegitimationstokens i stedet for delegerede kodeflowtokens.

- [Få adgang på vegne af brugere og delegerede tilladelser](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v2.0 – OAuth 2.0-godkendelseskodeflow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Få adgang uden en bruger (daemon-tjeneste) og programtilladelser](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v2.0 – OAuth 2.0 flow af legitimationsoplysninger](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**403 Forbudt fejl: Nulstilling af adgangskode**

Der er i øjeblikket ingen programtilladelses-daemon-tjeneste-til-tjeneste-tilladelser, der tillader nulstilling af brugeradgangskoder. Disse API'er understøttes kun ved hjælp af de interaktive delegerede kodeflows med en administrator, der er logget på.

- [Microsoft Graph-tilladelser](https://docs.microsoft.com/graph/permissions-reference)

**403 Forbudt: Har brugeren adgang, og har de licens?**

For delegerede kodeflows evaluerer Microsoft Graph, om anmodningen er tilladt på baggrund af de tilladelser, der er givet til appen, og de tilladelser, som brugeren, der er logget på, har. Generelt indikerer denne fejl, at brugeren ikke har rettigheder nok til at udføre anmodningen eller at brugeren ikke har licens til de data, der fås adgang til. Kun brugere med de nødvendige tilladelser eller licenser kan foretage anmodningen.

**403 Forbudt: Har du valgt den korrekte ressource-API?**

API-tjenester som Microsoft Graph kontrollerer, at aud-kravet (målgruppen) i den modtagne adgangstoken svarer til den værdi, det forventer for sig selv, og hvis ikke, medfører det en 403 Forbudt fejl. En almindelig fejl, der medfører denne fejl, er at forsøge at bruge en token, der er mortaget til Azure AD Graph APIs, Outlook APIs eller SharePoint/OneDrive APIs til at kalde Microsoft Graph (eller omvendt). Sørg for, at ressourcen (eller omfanget) din app henter et token for svarer til den API, som appen kalder.

**400 Forkert anmodning eller 403 Forbudt: Overholder brugeren organisationens politikker for betinget adgang (Conditional Access – CA) ?**

Baseret på en organisations nøglecenterpolitikker kan en bruger, der får adgang til Microsoft Graph-ressourcer via din app, blive kontaktet for yderligere oplysninger, der ikke findes i det adgangstoken, din app oprindeligt blev købt. I dette tilfælde modtager din app en 400 med en *interaction_required*-fejl under modtagelsen af adgangstoken 403 med *insufficient_claims*-fejl, når du kalder Microsoft Graph. I begge tilfælde indeholder fejlsvaret yderligere oplysninger, der kan præsenteres for godkendelsesslutpunktet for at give brugeren yderligere oplysninger (f.eks. multifaktorgodkendelse eller enhedsregistrering).

- [Håndtering af udfordringer med betinget adgang ved hjælp af MSAL ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Vejledning for udviklere om Azure Active Directory-betinget adgang](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
