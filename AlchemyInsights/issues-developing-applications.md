---
title: Problemer med udvikling af programmer
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
- "7754"
- "9004342"
ms.openlocfilehash: 065ff6d965063e44c4d1771821985058c9d020fbbabb0d381f30b6a11132c4ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013418"
---
# <a name="issues-developing-applications"></a>Problemer med udvikling af programmer

Hvis du vil foretage fejlfinding af de mest almindelige problemer med Azure Active Directory (AD), skal du se følgende artikler:

- [Jeg får kun vist problemer med at logge på programmer ved hjælp af Chrome-browseren](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Jeg ved ikke, hvordan jeg ændrer standardindstillingerne for tokenlevetid for mit program](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Jeg er forvirret over, hvordan samtykke til programmet fungerer](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Jeg ved ikke, hvordan jeg giver tilladelser til mit program](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Jeg forstår ikke forskellen mellem delegerede tilladelser og programtilladelser](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Ophør af support til Azure Active Directory Authentication Library (ADAL) og Azure AD Graph API (AAD Graph)***

- Fra d. 30. juni 2020 tilføjer vi ikke længere nye funktioner til ADAL (Azure Active Directory Authentication Library) og AAD Graph (Azure AD Graph API). Vi yder fortsat teknisk support og sikkerhedsopdateringer, men vil ikke længere levere funktionsopdateringer.

- Fra d. 30. juni 2022 afslutter vi supporten af ADAL og AAD Graph og yder ikke længere teknisk support eller sikkerhedsopdateringer. Som et resultat af denne betingelse er følgende konsekvenserne:

    - Apps, der bruger ADAL på eksisterende os-versioner, fungerer fortsat efter dette tidspunkt, men får ingen teknisk support eller sikkerhedsopdateringer.

    - Apps, der bruger AAD Graph efter dette tidspunkt, modtager muligvis ikke længere svar fra AAD Graph-slutpunktet

**ADAL-overførsel**

Hvis du bruger Microsoft-apps, anbefaler vi, at du opdaterer til Microsoft Authentication Library (MSAL), som har de nyeste funktioner og sikkerhedsopdateringer. Denne anbefaling er i forbindelse med, at Microsoft starter processen med at overføre sine apps til MSAL inden deadline for ophør af support. 

Microsofts overførsel af sine apps til MSAL sikrer, at appsene drager fordel af MSALs løbende sikkerheds- og funktionsforbedringer.

1. [Læs ofte stillede spørgsmål om ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Få mere at vide om at migrere apps pr. platform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Hvis du har brug for hjælp til at forstå, hvilke af dine apps der bruger ADAL, anbefaler vi, at du gennemser alle dine apps' kildekode og, hvis det er relevant, kontakt eventuelle uafhængige softwareleverandører eller appudbydere. Microsoft-support kan også give dig en liste over alle ikke-Microsoft ADAL-apps i din lejer.

**AAD Graph Migration**

For programmer, der bruger AAD Graph, skal du følge vores vejledning til at overføre AAD Graph apps til Microsoft Graph:

1. [Vores tjekliste til migrering indeholder et startpunkt](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. Din registreringsportal til Azure-app viser, hvilke programmer der bruger AAD Graph. Vi anbefaler, at du gennemgår alle dine apps kildekode og, hvis det er relevant, kontakt eventuelle uafhængige softwareleverandører eller appudbydere. Microsoft Support kan også give dig oplysninger om AAD Graph brug i din lejer.







