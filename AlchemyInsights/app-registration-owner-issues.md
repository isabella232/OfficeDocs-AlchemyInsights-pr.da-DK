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
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404453"
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
- Brug Azure AD-portalen – gå til [portal.azure.com](https://portal.azure.com/) > Azure Active Directory > Appregistrering > Vælg dit program > Ejere > Tilføj ejere

**Kan du ikke få vist dit program på bladet App-registreringer, selvom du er ejeren af det pågældende program?**

Ejeren af en app er ikke en administrativ rolle. Hvis indstillingen [Begræns adgang til Azure AD-administrationsportalen](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) er aktiveret, er det kun administratorer, der kan få vist programmerne på appregistreringsportalen. Hvis en ejer skal kunne få vist programmerne, skal du enten deaktivere denne indstilling (Angiv denne til NEJ) eller tildele administratorroller til ejeren kun for det specifikke program. Men til dette skal du bruge en Azure AD Premium P2-licens og aktivere administration af [privilegeret identitet.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)
