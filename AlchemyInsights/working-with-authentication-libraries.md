---
title: Arbejde med godkendelsesbiblioteker
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035288"
---
# <a name="working-with-authentication-libraries"></a>Arbejde med godkendelsesbiblioteker

Du kan løse problemet med Microsoft-godkendelsesbiblioteket (MSAL) ved at udføre følgende anbefalede trin:

1. **Arbejde med MSAL:** [Godkendelsesbiblioteker for Microsoft-identitetsplatformen](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) – Denne artikel viser understøttelse af Microsoft-godkendelsesbiblioteket for flere programtyper. Den indeholder links til bibliotekskildekode; hvor du kan hente pakken til din apps projekt; og om biblioteket understøtter brugeradgang (godkendelse), adgang til beskyttede web-API'er (godkendelse) eller begge dele.

2. **Fejlfinding af godkendelse:** MSAL understøtter flere godkendelsesflows til brug i forskellige programscenarier. Afhængigt af hvordan dit klientprogram er opbygget, kan MSAL bruge en eller flere af de godkendelsesflows, der understøttes af Microsoft-identitetsplatformen. Disse flows kan give flere typer tokens og godkendelseskoder og kræve forskellige tokens for at få dem til at fungere.

3. **Adgangstokens:** [Adgangstokens fra Microsoft-identitetsplatformen](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) – Få mere at vide om, hvordan din API kan validere og bruge krav i et adgangstoken. Al dokumentation i denne artikel, undtagen hvor den er angivet, gælder kun for tokens, der er udstedt for API'er, du har registreret. Den gælder ikke for tokens, der er udstedt for Microsoft-ejet API'er, og disse tokens kan heller ikke bruges til at validere, hvordan Microsoft-identitetsplatformen udsteder tokens for en API, du opretter.

**Ophør af understøttelse af Azure Active Directory Authentication Library (ADAL)**

- **Fra den 30. juni 2020** tilføjer vi ikke længere nye funktioner til ADAL og Azure AD Graph. Vi yder fortsat teknisk support og sikkerhedsopdateringer, men vil ikke længere levere funktionsopdateringer.
- **Fra d. 30. juni 2022** afslutter vi understøttelsen af ADAL og Azure AD Graph og yder ikke længere teknisk support eller sikkerhedsopdateringer.
- Apps, der bruger ADAL på eksisterende OS-versioner, fungerer fortsat efter dette tidspunkt, men får *ikke teknisk support eller sikkerhedsopdateringer.*
- Apps, der bruger Azure AD Graph efter dette tidspunkt, modtager muligvis ikke længere svar fra Azure AD Graph-slutpunktet.

**ADAL-overførsel**

- Vi anbefaler at opdatere til MSAL, som har de nyeste funktioner og sikkerhedsopdateringer.
- Hvis du bruger Microsoft-apps, skal du vide, at Microsoft er i gang med at overføre sine apps til MSAL inden slutdatoen for support, hvilket sikrer, at de får glæde af MSAL's løbende sikkerheds- og funktionsforbedringer.

1. [Læs ofte stillede spørgsmål om ADAL.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Få mere at vide om, hvordan du overfører apps på pr. platform.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance)
3. Hvis du efter at have læst vejledningen til din apps platform har yderligere spørgsmål, kan du skrive et opslag på [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) med mærket [azure-ad-adal-deprecation] eller åbne et problem i bibliotekets GitHub-lager. Se afsnittet Sprog og rammer i **MSAL-oversigtsartikel** for links til hvert [biblioteks](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) repo.
4. **Hvis du har brug for hjælp til at forstå, hvilke af** dine apps der bruger ADAL, anbefaler vi, at du gennemgår alle dine apps kildekode. Hvis det er relevant, skal du kontakte eventuelle uafhængige softwareleverandører eller appudbydere. Microsoft-support kan også give dig en liste over alle ikke-Microsoft ADAL-apps i din lejer.







