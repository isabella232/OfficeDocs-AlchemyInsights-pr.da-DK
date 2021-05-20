---
title: Opret bruger
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: 800baae2d748708d8cb7a5fb0e73fce5dcf455cb
ms.sourcegitcommit: 2d617ae59eed0ce8b571339ceefce6473c03b94c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/19/2021
ms.locfileid: "52569705"
---
# <a name="create-user"></a><span data-ttu-id="9473e-102">Opret bruger</span><span class="sxs-lookup"><span data-stu-id="9473e-102">Create user</span></span>

<span data-ttu-id="9473e-103">**MEDDELELSE:**</span><span class="sxs-lookup"><span data-stu-id="9473e-103">**ANNOUNCEMENT:**</span></span>

- <span data-ttu-id="9473e-104">[Udrådning af WebView-logonsupport fra Google fra den 4. januar 2021.](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support)</span><span class="sxs-lookup"><span data-stu-id="9473e-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) .</span></span> <span data-ttu-id="9473e-105">Test, om dine apps kan blive påvirket, ved [at følge Googles vejledning til](https://go.microsoft.com/fwlink/?linkid=2157323) test af kompatibilitet.</span><span class="sxs-lookup"><span data-stu-id="9473e-105">Test whether your apps may be affected by following [Google’s guidance](https://go.microsoft.com/fwlink/?linkid=2157323) on testing compatibility.</span></span>
- <span data-ttu-id="9473e-106">Sørg for at bruge systemwebvisningen eller systembrowseren, når du logger dine brugere på med Google-forbrugerkonti.</span><span class="sxs-lookup"><span data-stu-id="9473e-106">Make sure you use the system webview or system browser when signing in your users with consumer Google accounts.</span></span> <span data-ttu-id="9473e-107">Du kan få mere at vide [under Problemer med at logge på programmer, der kun bruger Chrome-browseren.](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)</span><span class="sxs-lookup"><span data-stu-id="9473e-107">For more information, see [Issues signing in to application(s) using Chrome browser only](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).</span></span>

<span data-ttu-id="9473e-108">**Jeg kan ikke oprette en ny bruger i mit Azure AD-katalog**</span><span class="sxs-lookup"><span data-stu-id="9473e-108">**I can't create a new user in my Azure AD directory**</span></span>

1. <span data-ttu-id="9473e-109">Sørg for, at du er godkendt til at oprette en ny standardbruger.</span><span class="sxs-lookup"><span data-stu-id="9473e-109">Ensure that you are authorized to create a new standard user.</span></span> <span data-ttu-id="9473e-110">Kun den globale administrator eller brugeradministratorrollen i Azure Active Directory (AD) kan oprette en ny standardbruger.</span><span class="sxs-lookup"><span data-stu-id="9473e-110">Only the Global administrator or User administrator role in Azure Active Directory (AD) can create a new standard user.</span></span> <span data-ttu-id="9473e-111">Hvis du ikke er i en af disse roller, kan du bede en administrator om at føje dig til en af disse roller eller oprette den nye brugerkonto for dig.</span><span class="sxs-lookup"><span data-stu-id="9473e-111">If you're not in one of these roles, ask an administrator to add you to one of these roles or to create the new user account for you.</span></span>
1. <span data-ttu-id="9473e-112">Sørg for, at brugernavnet er i et domæne, der er bekræftet i din Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9473e-112">Ensure that the user name is in a domain that is verified in your Azure AD.</span></span> <span data-ttu-id="9473e-113">Hvis du ikke har nogen bekræftede brugerdefinerede domænenavne i dit Azure AD, kan du bruge dit indledende Azure AD-domæne, som slutter med \*.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="9473e-113">If you do not have any verified custom domain names in your Azure AD, you can use your Azure AD initial domain, which ends with \*.onmicrosoft.com.</span></span>
1. <span data-ttu-id="9473e-114">Sørg for, at brugernavnet er i et domæne, der ikke er i organisationsnetværk med Azure AD fra dit lokale AD.</span><span class="sxs-lookup"><span data-stu-id="9473e-114">Ensure that the user name is in a domain that is not federated to Azure AD from your on-premises AD.</span></span> <span data-ttu-id="9473e-115">Brugere kan ikke tilføjes i skyen med domænenavne, der er medlem af organisationsnetværket i det lokale miljø.</span><span class="sxs-lookup"><span data-stu-id="9473e-115">Users cannot be added in the cloud with domain names that are federated from on-premises.</span></span>
1. <span data-ttu-id="9473e-116">Sørg for, at ingen andre brugere eller kontakter allerede har det brugernavn, du vil tildele den nye bruger.</span><span class="sxs-lookup"><span data-stu-id="9473e-116">Ensure that no other user or contact already has the user name that you want to assign to the new user.</span></span> <span data-ttu-id="9473e-117">Brugernavne skal være entydige på tværs af Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9473e-117">User names must be unique across Azure AD.</span></span>
1. <span data-ttu-id="9473e-118">Se [Roller og administratorer i Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) AD for dit Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9473e-118">See [Azure AD roles and administrators](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="9473e-119">Se [domænenavnene til](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) dit Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9473e-119">See the [domain names](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="9473e-120">Gennemse [overvågningslogfiler for at](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) få vist mere detaljerede oplysninger om en nyligt oprettet eller slettet bruger, som f.eks. hvem der udførte handlingen og hvornår.</span><span class="sxs-lookup"><span data-stu-id="9473e-120">Review [Audit logs](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) to see more detailed information about a recently created or deleted user like who performed the action and when.</span></span>
1. <span data-ttu-id="9473e-121">Du kan finde flere oplysninger om at tilføje nye brugere [i Brug Azure-portalen til at oprette en ny bruger i dit Azure AD](/azure/active-directory/active-directory-users-create-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="9473e-121">For more information on adding new users, see [Use the Azure portal to create a new user in your Azure AD](/azure/active-directory/active-directory-users-create-azure-portal).</span></span>
1. <span data-ttu-id="9473e-122">[Administrative roller i Azure AD:](/azure/active-directory/active-directory-assign-admin-roles)Administratorrolletilladelser i Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="9473e-122">[Azure AD administrative roles](/azure/active-directory/active-directory-assign-admin-roles): Administrator role permissions in Azure Active Directory</span></span>
1. <span data-ttu-id="9473e-123">Du kan også [bruge Azure AD PowerShell til at oprette en ny bruger.](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="9473e-123">You can also [use Azure AD PowerShell to create a new user](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).</span></span>
