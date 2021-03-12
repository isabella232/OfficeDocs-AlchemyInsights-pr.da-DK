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
ms.openlocfilehash: 9c37ad8e4dfecdb59a37d767f8eb4a5d99be7fa1
ms.sourcegitcommit: d13f23fb7994871d4e0e6e3e43672a101bd779e8
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/28/2021
ms.locfileid: "50713447"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Problemer med en ressource eller tjenesteinspektør

1. Hvis du kun lige er begyndt, beskriver [Application and Service Principal Objects](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) i Azure Active Directory programregistrering, programobjekter og tjeneste principaler i Azure Active Directory: hvad de er, hvordan de bruges, og hvordan de er relateret til hinanden. Der præsenteres også et eksempelscenarie med flere lejere for at illustrere relationen mellem et programs programobjekt og tilsvarende tjeneste hovedobjekter.
2. Du kan få mere at vide om relationen mellem programmer og tjeneste principaler ved at læse [programmer og tjeneste hovedobjekter i Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
3. [Sådan gør du:](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) Brug portalen til at oprette et Azure AD-program og en tjenesteinspektør, der kan få adgang til ressourcer, viser dig, hvordan du opretter et nyt Azure Active Directory-program (Azure AD) og en tjenesteinspektør, der kan bruges sammen med det rollebaserede adgangskontrolelement.
4. Med tjenestens [hoved-API](https://docs.microsoft.com/graph/api/resources/serviceprincipal)kan du programmeringligt administrere forekomster af programmer og styre, hvad et program kan gøre i din lejer.
5. [servicePrincipal-ressourcetypen](https://docs.microsoft.com/graph/api/resources/serviceprincipal) viser alle egenskaber og metoder for servicePrincipal-ressourcetypen.
6. [Forskelle i ressourcetyper mellem Azure AD Graph og Microsoft Graph fremhæver](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) forskellene mellem Azure AD Graph- og Microsoft Graph-ressourcer. Den viser ressourcer, der har forskellige navne eller ikke er tilgængelige. den fremhæver også de ressourcer, der er tilgængelige i betaversionen af Microsoft Graph, men ikke i versionen v1.0.

**Problemer med gæstebrugere**

- [Hurtig start:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) Føj gæstebrugere til dit katalog i Azure-portalen viser dig, hvordan du føjer en ny gæstebruger til dit Azure AD-katalog via Azure-portalen, sender en invitation og ser, hvordan gæstebrugerens indløsningsproces ser ud.
- [Selvstudium: Opret brugerflows i Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) viser, hvordan du opretter nogle anbefalede brugerflows ved hjælp af Azure-portalen. Hvis du leder efter oplysninger om, hvordan du konfigurerer flowet for legitimationsoplysninger for en ressourceejers adgangskode (ROPC) i dit program, skal du se Konfigurere flowet til legitimationsoplysninger for ressourceejerens adgangskode i Azure AD B2C.
