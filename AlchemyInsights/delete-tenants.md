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
ms.openlocfilehash: 7377f77b7295e8134673c9a46fa7606842d4df949f535878d13986c6d39d0b5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53993887"
---
# <a name="delete-tenant"></a>Slet lejer

Hvis du vil slette et Azure AD, skal du sikre dig, at:
- Du er global administrator i kataloget.
- Du er IKKE logget på med en konto, der har standardmappen, f.eks. contoso.onmicrosoft.com på kontoen, der er logget på, f.eks. admin@contoso.onmicrosoft.com.
- Fjern alle aktive programmer i mappen før sletning. Hvis du vil fjerne aktive programmer, skal du gå til App-registreringer og fjerne de eksisterende programmer.
- Der er ingen aktive abonnementer på nogen Microsoft-onlinetjenester, f.eks. Microsoft Azure, Office 365 eller Azure AD Premium, der er knyttet til kataloget. Overfør dine abonnementer eller fremskyndet annullering af aktive abonnementer via Azure Support og fakturering. Få mere at vide om, hvordan du annullerer Office 365 og Azure-abonnementer. Du kan finde en vejledning til tilknytning eller tilføjelse af et eksisterende abonnement til en lejer under Tilknyt eller føj et [Azure-abonnement til din Azure AD-lejer.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)
- Der er ingen aktiv licens. Hvis du vil fjerne licenser, skal [du se Sådan fjerner du Abonnement på at fjerne licens](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- Der er ingen andre aktive brugere i kataloget end dig selv som global administrator, når du forsøger at slette Azure AD. Fjern alle andre aktive brugere, og eventuelle afhængigheder af et brugerdefineret domænenavn i lejeren skal også fjernes, f.eks. brugere, der er oprettet med admin@contoso.com.

Hvis du vil have mere at vide om, hvordan du:
- Slet "Azure Active Directory" eller "abonnement" i [Slet Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Hvis du vil fjerne programmer i mappen, skal du [se Fjerne programmer](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
