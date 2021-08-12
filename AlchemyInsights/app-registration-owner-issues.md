---
title: Problemer med appregistreringsejer
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9655"
ms.openlocfilehash: cd7533f09ed8361e134b81979532cdebbf49971c54553a0172c7527f30e319bb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951127"
---
# <a name="app-registration-owner-issues"></a>Problemer med appregistreringsejer

Følgende er de tilgængelige metoder til at tilføje hovedstolen som ejere for appregistreringer:

- Brug af Azure AD PowerShell-modul -

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    Reference: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Brug af Azure CLI - `az ad app owner add`

    Reference: [az ad app-ejer](https://docs.microsoft.com/cli/azure/ad/app/owner)
- Brug af MS Graph -

    Reference: [Tilføj ejer – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- Brug Azure AD-portalen – Gå til [portal.azure.com](https://portal.azure.com/) > Azure Active Directory > Appregistrering > Vælg dit program > Ejere > Tilføj ejere

**Kan du ikke få vist dit program på bladet til appregistrering, selvom du er ejeren af det pågældende program?**

Ejer af en app er ikke en administrativ rolle. Hvis indstillingen [Begræns adgang til Azure AD-administrationsportalen](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) er aktiveret, er det kun administratorer, der vil kunne få vist programmerne på appregistreringsportalen. Hvis en ejer skal kunne få vist programmerne, skal du enten deaktivere denne indstilling (Angiv denne til NEJ) eller tildele administratorroller til ejeren kun for det specifikke program. Men til dette skal du have en Azure AD Premium P2-licens og aktivere [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).
