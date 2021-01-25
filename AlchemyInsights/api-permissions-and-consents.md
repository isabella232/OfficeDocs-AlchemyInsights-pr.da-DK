---
title: API-tilladelser og-samtykke
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
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974371"
---
# <a name="api-permissions-and-consent"></a><span data-ttu-id="bb59b-102">API-tilladelser og-samtykke</span><span class="sxs-lookup"><span data-stu-id="bb59b-102">API permissions and consent</span></span>

<span data-ttu-id="bb59b-103">Programmer, der integreres med Microsoft Identity platform, følger en godkendelsesmodel, der giver brugere og administratorer kontrol over, hvordan data kan åbnes.</span><span class="sxs-lookup"><span data-stu-id="bb59b-103">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="bb59b-104">Implementeringen af godkendelses modellen er blevet opdateret på Microsoft Identity platform Endpoint.</span><span class="sxs-lookup"><span data-stu-id="bb59b-104">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint.</span></span> <span data-ttu-id="bb59b-105">Det ændrer, hvordan en app skal interagere med Microsoft Identity platform.</span><span class="sxs-lookup"><span data-stu-id="bb59b-105">It changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="bb59b-106">[Tilladelser og samtykke i Microsoft Identity platform Endpoint](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) dækker de grundlæggende begreber for denne godkendelsesmodel, herunder områder, tilladelser og samtykke.</span><span class="sxs-lookup"><span data-stu-id="bb59b-106">[Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) covers the basic concepts of this authorization model, including scopes, permissions, and consent.</span></span>

<span data-ttu-id="bb59b-107">[Azure Active Directory (Azure ad)-samtykke Framework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) gør det nemt at udvikle Internet-og oprindelige klientprogrammer fra flere arkitekturer.</span><span class="sxs-lookup"><span data-stu-id="bb59b-107">The [Azure Active Directory (Azure AD) consent framework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) makes it easy to develop multi-tenant web and native client applications.</span></span> <span data-ttu-id="bb59b-108">Disse programmer tillader, at der logges af brugerkonti fra en Azure AD-lejer, der er anderledes end den, hvor programmet er registreret.</span><span class="sxs-lookup"><span data-stu-id="bb59b-108">These applications allow sign-in by user accounts from an Azure AD tenant that's different from the one where the application is registered.</span></span> <span data-ttu-id="bb59b-109">De kan også have brug for at få adgang til webapi'er som Microsoft Graph API (for at få adgang til Azure AD, Intune og tjenester i Microsoft 365) og andre Microsoft-tjenesters API'er, ud over dine egne webapi'er.</span><span class="sxs-lookup"><span data-stu-id="bb59b-109">They may also need to access web APIs such as the Microsoft Graph API (to access Azure AD, Intune, and services in Microsoft 365) and other Microsoft services' APIs, in addition to your own web APIs.</span></span>

