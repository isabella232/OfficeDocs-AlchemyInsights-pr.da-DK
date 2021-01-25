---
title: Problemer med at udvikle programmer med API'er
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
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974379"
---
# <a name="issues-developing-applications-with-apis"></a>Problemer med at udvikle programmer med API'er

Du kan komme i gang med at bruge Azure Active Directory-graf-API'ET ved at se vejledning til hurtig start til [Azure ad Graph](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) eller få vist den [interaktive referencedokumentation til Azure ad Graph-API](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).

**Afslutning af understøttelse af Azure Active Directory-godkendelses bibliotek (ADAL) og Azure AD Graph API (AAD-graf)**

**Starter Juni 30th, 2020**, vil vi ikke længere tilføje nye funktioner til ADAL og Azure ad Graph. Vi vil fortsat yde teknisk support og sikkerhedsopdateringer, men vil ikke længere tilbyde FUNKTIONSOPDATERINGER.

**Fra og med juni 30th, 2022**, vi slutter support til ADAL og Azure ad Graph og vil ikke længere yde teknisk support eller sikkerhedsopdateringer.

Apps, der bruger ADAL på eksisterende OS-versioner, vil fortsat fungere efter dette tidspunkt, men de får ikke teknisk support eller sikkerhedsopdateringer.

Apps, der bruger Azure AD Graph efter dette tidspunkt, kan muligvis ikke længere modtage svar fra Azure AD Graph-slutpunktet.

**ADAL-overførsel**

Vi anbefaler, at du opdaterer til [Microsoft-godkendelses bibliotek (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), som har de nyeste funktioner og sikkerhedsopdateringer.

Hvis du bruger Microsoft-apps, skal du vide, at Microsoft er i gang med at overføre sine programmer til MSAL ved hjælp af deadline for sidste support, så de kan drage fordel af MSAL de vedvarende sikkerheds-og funktionsforbedringer.

1. [Læs ADAL ofte stillede spørgsmål](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. [Få mere at vide om, hvordan du kan overføre apps på et enkelt platforms grundlag](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. Hvis du har brug for hjælp til at forstå, hvilke af dine apps der bruger ADAL, anbefaler vi, at du gennemgår alle dine apps-kildekode, og hvis det er relevant, kan du få adgang til alle ISV'er-eller app-udbydere. Microsoft Support kan også give dig en liste over alle ikke-Microsoft-ADAL-apps i din lejer.

**AAD-diagram overførsel**

For programmer, der bruger Azure AD Graph, skal du følge vores vejledning til at overføre [Azure ad Graph-apps til Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).

1. [Vores overflytnings checkliste giver et](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)introduktions point. 
1. Din Azure-app-registrerings Portal viser, hvilke programmer der bruger AAD-grafer. Vi anbefaler, at du gennemgår alle din apps-kildekode, og hvis det er relevant, så du kan få adgang til alle ISV'er-eller app-udbydere. Microsoft Support kan også give dig en liste over alle AAD-diagram brug i din lejer.
1. Hvis din app skal have adgang til data i Microsoft Graph, skal brugeren eller administratoren give den de rette tilladelser via en tilladelses proces. [Microsoft Graph-tilladelses referencen](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) viser de tilladelser, der er knyttet til hvert omfattende sæt Microsoft Graph-API'er. Den indeholder også en vejledning til, hvordan du brugertilladelserne.
