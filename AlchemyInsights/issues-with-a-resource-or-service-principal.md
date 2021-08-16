---
title: Problemer med en ressource eller tjenesteinspektør
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
- "9004336"
- "7741"
ms.openlocfilehash: 52b9b2e950d66c2f4105b76c4e2c70ed51320e4a57eb0008c353a9587fcc6510
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028070"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Problemer med en ressource eller tjenesteinspektør

1. Hvis du lige er begyndt, beskriver [Application and service principal objects](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) i Azure Active Directory programregistrering, programobjekter og tjeneste principaler i Azure Active Directory: hvad de er, hvordan de bruges, og hvordan de er relateret til hinanden. Der vises også et eksempelscenarie med flere lejere til at illustrere relationen mellem et programs programobjekt og tilsvarende tjeneste hovedobjekter.
2. Du kan få mere at vide om relationen mellem programmer og tjenesteinspektører ved at læse programmer og [tjeneste hovedobjekter i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).
3. [Sådan gør du:](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) Brug portalen til at oprette et Azure AD-program og en tjenesteinspektør, der kan få adgang til ressourcer, viser, hvordan du opretter et nyt Azure Active Directory-program (Azure AD) og tjeneste principal, der kan bruges med den rollebaserede adgangskontrol.
4. Med tjenestens [hoved-API](https://docs.microsoft.com/graph/api/resources/serviceprincipal)kan du ved hjælp af programmering administrere forekomster af programmer og styre, hvad et program kan gøre i din lejer.
5. [servicePrincipal-ressourcetype](https://docs.microsoft.com/graph/api/resources/serviceprincipal) viser alle egenskaber og metoder for servicePrincipal-ressourcetypen.
6. [Forskelle på ressourcetyper mellem Azure AD Graph og Microsoft Graph fremhæver](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) forskellene mellem Azure AD Graph og Microsoft Graph ressourcer. Den viser ressourcer, der har forskellige navne eller ikke er tilgængelige. den fremhæver også de ressourcer, der er tilgængelige i betaversionen af Microsoft Graph men ikke i versionen v1.0.

**Problemer med gæstebrugere**

- [Hurtig start:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) Føj gæstebrugere til dit katalog i Azure-portalen viser dig, hvordan du kan føje en ny gæstebruger til dit Azure AD-katalog via Azure-portalen, sende en invitation og se, hvordan gæstebrugerens indløsningsproces ser ud.
- [Selvstudium: Opret brugerflows i Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) viser, hvordan du opretter nogle anbefalede brugerflows ved hjælp af Azure-portalen. Hvis du leder efter oplysninger om, hvordan du konfigurerer flowet for legitimationsoplysninger for en ressourceejers adgangskode i dit program, skal du se Konfigurere flowet for legitimationsoplysninger for ressourceejerens adgangskode i Azure AD B2C.
