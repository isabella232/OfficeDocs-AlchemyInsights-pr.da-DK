---
title: Slet lejer
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564487"
---
# <a name="delete-tenant"></a>Slet lejer

Hvis du vil slette en Azure AD, skal du sikre:
- Du er Global administrator på adresselisten.
- Du er ikke logget på med en konto, der har standardmappen som f. eks contoso.onmicrosoft.com på den konto, der er logget på, f. eks admin@contoso.onmicrosoft.com.
- Fjern eventuelle aktive programmer i kataloget, før de slettes. Hvis du vil fjerne aktive programmer, skal du gå til App-registreringer og fjerne eksisterende programmer.
- Der er ingen aktive abonnementer til Microsoft online-tjenester, såsom Microsoft Azure, Office 365 eller Azure AD Premium, der er knyttet til kataloget. Overfør dine abonnementer, eller fremskyndelse af aktive abonnementer via Azure support og fakturering. Få mere at vide om, hvordan du annullerer Office 365 og Azure-abonnementer. Du kan finde en vejledning til, hvordan du knytter eller tilføjer et eksisterende abonnement til en lejer, under [tilknytte eller tilføje et Azure-abonnement til din Azure ad-lejer](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).
- Der er ingen aktiv licens. Hvis du vil fjerne licenser, skal du se [Sådan fjerner du abonnementet for at fjerne licensen](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- Der er ingen andre aktive brugere i oversigten ud over selv som den globale administrator, når de forsøger at slette Azure AD. Fjern eventuelle andre aktive brugere, og afhængigheder på et brugerdefineret domænenavn i lejeren skal også fjernes, f. eks brugere oprettet med admin@contoso.com.

Du kan finde flere oplysninger om, hvordan du gør følgende:
- Slet "Azure Active Directory" eller "abonnement", se [Slet Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Hvis du vil fjerne programmer i mappen, skal du se [fjerne programmer](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
