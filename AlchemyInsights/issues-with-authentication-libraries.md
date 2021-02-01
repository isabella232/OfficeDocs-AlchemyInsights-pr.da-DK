---
title: Problemer med godkendelsesbiblioteker
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
- "9004333"
- "7731"
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063589"
---
# <a name="issues-with-authentication-libraries"></a><span data-ttu-id="b01b1-102">Problemer med godkendelsesbiblioteker</span><span class="sxs-lookup"><span data-stu-id="b01b1-102">Issues with Authentication Libraries</span></span>

1. <span data-ttu-id="b01b1-103">[Godkendelsesbiblioteker for Microsoft-identitetsplatformen](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) viser microsoft-understøttede og kompatible klient- og middlewarebiblioteker.</span><span class="sxs-lookup"><span data-stu-id="b01b1-103">[Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) lists Microsoft-supported and compatible client and middleware libraries.</span></span>
2. <span data-ttu-id="b01b1-104">Microsoft Authentication Library (MSAL) understøtter flere [godkendelsesflows](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) til brug i forskellige programscenarier.</span><span class="sxs-lookup"><span data-stu-id="b01b1-104">The Microsoft Authentication Library (MSAL) supports several [authentication flows](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) for use in different application scenarios.</span></span>
3. <span data-ttu-id="b01b1-105">For at godkende og anskaffe tokens skal du initialisere et nyt offentligt eller fortroligt klientprogram i din kode.</span><span class="sxs-lookup"><span data-stu-id="b01b1-105">To authenticate and acquire tokens, you initialize a new public or confidential client application in your code.</span></span> <span data-ttu-id="b01b1-106">Du kan angive flere konfigurationsindstillinger, når du initialiserer klientappen i Microsoft-godkendelsesbiblioteket (MSAL).</span><span class="sxs-lookup"><span data-stu-id="b01b1-106">You can set several configuration options when you initialize the client app in the Microsoft Authentication Library (MSAL).</span></span> <span data-ttu-id="b01b1-107">Du kan få mere at vide under [Indstillinger for programkonfiguration.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)</span><span class="sxs-lookup"><span data-stu-id="b01b1-107">To learn more, see [Application configuration options](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span></span>

<span data-ttu-id="b01b1-108">**Ophør af understøttelse af Azure Active Directory Authentication Library (ADAL) og Azure AD Graph API (AAD Graph)**</span><span class="sxs-lookup"><span data-stu-id="b01b1-108">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="b01b1-109">**Fra den 30. juni 2020** tilføjer vi ikke længere nye funktioner til ADAL og Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="b01b1-109">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="b01b1-110">Vi yder fortsat teknisk support og sikkerhedsopdateringer, men vil ikke længere levere funktionsopdateringer.</span><span class="sxs-lookup"><span data-stu-id="b01b1-110">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="b01b1-111">**Fra den 30. juni 2022** afslutter vi understøttelsen af ADAL og Azure AD Graph og yder ikke længere teknisk support eller sikkerhedsopdateringer.</span><span class="sxs-lookup"><span data-stu-id="b01b1-111">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="b01b1-112">Apps, der bruger ADAL på eksisterende os-versioner, vil fortsat fungere efter dette tidspunkt, men vil *ikke få teknisk support eller sikkerhedsopdateringer.*</span><span class="sxs-lookup"><span data-stu-id="b01b1-112">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="b01b1-113">Apps, der bruger Azure AD Graph efter dette tidspunkt, modtager muligvis ikke længere svar fra Azure AD Graph-slutpunktet.</span><span class="sxs-lookup"><span data-stu-id="b01b1-113">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="b01b1-114">**ADAL-overførsel**</span><span class="sxs-lookup"><span data-stu-id="b01b1-114">**ADAL Migration**</span></span>

<span data-ttu-id="b01b1-115">Vi anbefaler, at du opdaterer [MSAL (Microsoft Authentication Library)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), som har de nyeste funktioner og sikkerhedsopdateringer.</span><span class="sxs-lookup"><span data-stu-id="b01b1-115">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="b01b1-116">Hvis du bruger Microsoft-apps, skal du vide, at Microsoft er i gang med at overføre sine programmer til MSAL inden slutdatoen for support, hvilket sikrer, at de får glæde af MSAL's løbende sikkerheds- og funktionsforbedringer.</span><span class="sxs-lookup"><span data-stu-id="b01b1-116">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they will benefit from MSAL's ongoing security and feature improvements.</span></span>

<span data-ttu-id="b01b1-117">Du kan finde flere oplysninger under:</span><span class="sxs-lookup"><span data-stu-id="b01b1-117">For more information, see:</span></span>

1. [<span data-ttu-id="b01b1-118">Læs ofte stillede spørgsmål om ADAL</span><span class="sxs-lookup"><span data-stu-id="b01b1-118">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="b01b1-119">Få mere at vide om at migrere apps pr. platform</span><span class="sxs-lookup"><span data-stu-id="b01b1-119">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="b01b1-120">Hvis du har brug for hjælp til at forstå, hvilke af dine apps der bruger ADAL, anbefaler vi, at du gennemgår alle dine apps kildekode og, hvis det er relevant, tager kontakt til eventuelle internetudbydere eller appudbydere.</span><span class="sxs-lookup"><span data-stu-id="b01b1-120">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="b01b1-121">Microsoft-support kan også give dig en liste over alle ikke-Microsoft ADAL-apps i din lejer.</span><span class="sxs-lookup"><span data-stu-id="b01b1-121">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="b01b1-122">**AAD Graph Migration**</span><span class="sxs-lookup"><span data-stu-id="b01b1-122">**AAD Graph Migration**</span></span>

<span data-ttu-id="b01b1-123">For programmer, der bruger Azure AD Graph, skal du følge vores vejledning til [at overføre Azure AD Graph-apps til Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)</span><span class="sxs-lookup"><span data-stu-id="b01b1-123">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. [<span data-ttu-id="b01b1-124">Vores tjekliste til overførsel giver et introduktionspunkt.</span><span class="sxs-lookup"><span data-stu-id="b01b1-124">Our migration checklist provides a getting started point.</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. <span data-ttu-id="b01b1-125">Din registreringsportal til Azure-app viser, hvilke programmer der bruger AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="b01b1-125">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="b01b1-126">Vi anbefaler, at du gennemser kildekoden til alle dine apps og, hvis det er relevant, skal du kontakte alle internetudbydere eller appudbydere.</span><span class="sxs-lookup"><span data-stu-id="b01b1-126">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="b01b1-127">Microsoft Support kan også give dig en liste over al AAD Graph-brug i din lejer.</span><span class="sxs-lookup"><span data-stu-id="b01b1-127">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="b01b1-128">For at din app kan få adgang til data i Microsoft Graph, skal brugeren eller administratoren give den de rette tilladelser via en samtykkeproces.</span><span class="sxs-lookup"><span data-stu-id="b01b1-128">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="b01b1-129">[Tilladelsesreferencen for Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) viser de tilladelser, der er knyttet til hvert overordnede sæt af Microsoft Graph-API'er.</span><span class="sxs-lookup"><span data-stu-id="b01b1-129">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="b01b1-130">Den indeholder også en vejledning til, hvordan du bruger tilladelserne.</span><span class="sxs-lookup"><span data-stu-id="b01b1-130">It also provides guidance about how to use the permissions.</span></span>
