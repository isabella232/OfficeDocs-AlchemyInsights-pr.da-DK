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
# <a name="app-registration-owner-issues"></a><span data-ttu-id="a07bf-102">Problemer med appregistreringsejer</span><span class="sxs-lookup"><span data-stu-id="a07bf-102">App Registration Owner issues</span></span>

<span data-ttu-id="a07bf-103">Følgende er de tilgængelige metoder til at tilføje hovedstolen som ejere for appregistreringer:</span><span class="sxs-lookup"><span data-stu-id="a07bf-103">Following are the available methods to add principals as owners for app registrations:</span></span>

- <span data-ttu-id="a07bf-104">Brug af Azure AD PowerShell-modul -</span><span class="sxs-lookup"><span data-stu-id="a07bf-104">Using Azure AD PowerShell Module -</span></span>

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    <span data-ttu-id="a07bf-105">Reference: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span><span class="sxs-lookup"><span data-stu-id="a07bf-105">Reference: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span></span>
- <span data-ttu-id="a07bf-106">Brug af Azure CLI - `az ad app owner add`</span><span class="sxs-lookup"><span data-stu-id="a07bf-106">Using Azure CLI - `az ad app owner add`</span></span>

    <span data-ttu-id="a07bf-107">Reference: [az ad app-ejer](https://docs.microsoft.com/cli/azure/ad/app/owner)</span><span class="sxs-lookup"><span data-stu-id="a07bf-107">Reference: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span></span>
- <span data-ttu-id="a07bf-108">Brug af MS Graph -</span><span class="sxs-lookup"><span data-stu-id="a07bf-108">Using MS Graph -</span></span>

    <span data-ttu-id="a07bf-109">Reference: [Tilføj ejer – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span><span class="sxs-lookup"><span data-stu-id="a07bf-109">Reference: [Add owner - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span></span>
- <span data-ttu-id="a07bf-110">Brug Azure AD-portalen – gå til [portal.azure.com](https://portal.azure.com/) > Azure Active Directory > Appregistrering > Vælg dit program > Ejere > Tilføj ejere</span><span class="sxs-lookup"><span data-stu-id="a07bf-110">Using the Azure AD Portal - Navigate to [portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Select your application > Owners > Add Owners</span></span>

<span data-ttu-id="a07bf-111">**Kan du ikke få vist dit program på bladet App-registreringer, selvom du er ejeren af det pågældende program?**</span><span class="sxs-lookup"><span data-stu-id="a07bf-111">**Cannot view your application on App Registrations blade even though you are the owner of that application?**</span></span>

<span data-ttu-id="a07bf-112">Ejeren af en app er ikke en administrativ rolle.</span><span class="sxs-lookup"><span data-stu-id="a07bf-112">Owner of an app is not an administrative role.</span></span> <span data-ttu-id="a07bf-113">Hvis indstillingen [Begræns adgang til Azure AD-administrationsportalen](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) er aktiveret, er det kun administratorer, der kan få vist programmerne på appregistreringsportalen.</span><span class="sxs-lookup"><span data-stu-id="a07bf-113">If the setting [Restrict access to Azure AD administration portal](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) is enabled, then only admin will be able to view the applications on App Registration portal.</span></span> <span data-ttu-id="a07bf-114">Hvis en ejer skal kunne få vist programmerne, skal du enten deaktivere denne indstilling (Angiv denne til NEJ) eller tildele administratorroller til ejeren kun for det specifikke program.</span><span class="sxs-lookup"><span data-stu-id="a07bf-114">For an owner to be able to view the applications, either disable this setting (Set this to NO) or assign admin role to the owner for only the specific application.</span></span> <span data-ttu-id="a07bf-115">Men til dette skal du bruge en Azure AD Premium P2-licens og aktivere administration af [privilegeret identitet.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)</span><span class="sxs-lookup"><span data-stu-id="a07bf-115">However for this, you will require an Azure AD Premium P2 license and enable [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span></span>
