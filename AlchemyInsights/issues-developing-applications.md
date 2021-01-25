---
title: Problemer med at udvikle programmer
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
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974306"
---
# <a name="issues-developing-applications"></a>Problemer med at udvikle programmer

Hvis du vil foretage fejlfinding af de mest almindelige problemer ved oprettelse af Azure Active Directory (AD)-apps, skal du se følgende artikler:

- [Jeg kan se problemer med at logge på programmer ved hjælp af Chrome-browser](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Jeg ved ikke, hvordan du ændrer standarderne for token-levetid for mit program](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Jeg er usikker på, hvordan program samtykke fungerer](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Jeg ved ikke, hvordan jeg giver tilladelse til mit program](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Jeg forstår ikke forskellen mellem delegerede og program tilladelser](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Slutningen af understøttelse af Azure Active Directory-godkendelses bibliotek (ADAL) og Azure ad Graph API (Aad-graf)** _

- Fra juni 30th, 2020, vil vi ikke længere tilføje nye funktioner til Azure Active Directory-godkendelses bibliotek (ADAL) og Azure AD graf API (AAD-graf). Vi vil fortsat yde teknisk support og sikkerhedsopdateringer, men vil ikke længere tilbyde FUNKTIONSOPDATERINGER.

- Fra juni 30th, 2022, vi afslutter support til ADAL og AAD-grafen og vil ikke længere yde teknisk support eller sikkerhedsopdateringer. Som følge af denne betingelse gælder følgende:

    - Apps, der bruger ADAL på eksisterende OS-versioner, vil fortsat fungere efter dette tidspunkt, men de får ikke teknisk support eller sikkerhedsopdateringer.

    - Apps, der bruger AAD Graph efter dette tidspunkt, kan muligvis ikke længere modtage svar fra det AAD-diagram slutpunkt

_ *ADAL-overførsel**

Hvis du bruger Microsoft-apps, anbefaler vi, at du opdaterer til Microsoft-godkendelses bibliotek (MSAL), som har de nyeste funktioner og sikkerhedsopdateringer. Denne anbefaling er i forbindelse med Microsoft, der starter processen med at overføre sine apps til MSAL ved hjælp af deadline for support. 

Overførslen af Microsofts apps til MSAL sikrer, at apps nyder godt af de vedvarende sikkerheds-og funktionsforbedringer for MSAL.

1. [Læs ADAL ofte stillede spørgsmål](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Få mere at vide om, hvordan du kan overføre apps på et enkelt platforms grundlag](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Hvis du har brug for hjælp til at forstå, hvilke af dine apps der bruger ADAL, anbefaler vi, at du gennemgår alle dine apps-kildekode, og hvis det er relevant, at få adgang til uafhængige softwareleverandører eller app-udbydere. Microsoft Support kan også give dig en liste over alle ikke-Microsoft-ADAL-apps i din lejer.

**AAD-diagram overførsel**

For programmer, der bruger AAD-graf, skal du følge vores vejledning til at overføre AAD-apps til Microsoft Graph:

1. [Vores overflytnings checkliste giver et](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)introduktions point. 
2. Din Azure-app-registrerings Portal viser, hvilke programmer der bruger AAD-grafer. Vi anbefaler, at du gennemgår alle dine apps-kildekoder, og hvis det er relevant, at få adgang til uafhængige softwareleverandører eller app-udbydere. Microsoft Support kan også give dig oplysninger om AAD-diagram brug i din lejer.







