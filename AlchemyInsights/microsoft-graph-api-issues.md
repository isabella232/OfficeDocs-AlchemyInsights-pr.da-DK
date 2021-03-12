---
title: Problemer med Microsoft Graph API
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
- "9004345"
- "7759"
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/29/2021
ms.locfileid: "50713471"
---
# <a name="microsoft-graph-api-issues"></a><span data-ttu-id="08d95-102">Problemer med Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="08d95-102">Microsoft Graph API issues</span></span>

<span data-ttu-id="08d95-103">Dette emne kan også gælde for udviklere, der stadig bruger Azure AD Graph API.</span><span class="sxs-lookup"><span data-stu-id="08d95-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="08d95-104">Det anbefales dog på **det kraftigste,** at du bruger Microsoft Graph til alle scenarierne administration af katalog, identitet og adgang.</span><span class="sxs-lookup"><span data-stu-id="08d95-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="08d95-105">**Godkendelses- eller godkendelsesproblemer**</span><span class="sxs-lookup"><span data-stu-id="08d95-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="08d95-106">Hvis din app ikke kan få **tokens** til at kalde Microsoft Graph, skal du vælge Problem med at få en adgangstoken **(godkendelse)** kategori for Microsoft Graph for at få mere specifik hjælp og support til dette emne.</span><span class="sxs-lookup"><span data-stu-id="08d95-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="08d95-107">Hvis din app modtager **401-** eller 403-godkendelsesfejl, når du kalder Microsoft Graph, skal du vælge kategorien Få en adgang nægtet-fejl **(Godkendelse)** Microsoft Graph API for at få mere specifik hjælp og support i dette emne.</span><span class="sxs-lookup"><span data-stu-id="08d95-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="08d95-108">**Jeg vil bruge Microsoft Graph, men jeg er ikke sikker på, hvor jeg skal starte**</span><span class="sxs-lookup"><span data-stu-id="08d95-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

- [<span data-ttu-id="08d95-109">Oversigt over Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="08d95-109">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="08d95-110">Oversigt over identitets- og adgangsstyring i Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="08d95-110">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="08d95-111">Introduktion til at bygge Microsoft Graph-apps</span><span class="sxs-lookup"><span data-stu-id="08d95-111">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="08d95-112">**Microsoft Graph Explorer** – Test Microsoft Graph-API'er i din lejer eller en demolejer</span><span class="sxs-lookup"><span data-stu-id="08d95-112">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="08d95-113">**Jeg vil bruge Microsoft Graph, men understøtter den de v1.0-mappe-API'er, jeg har brug for?**</span><span class="sxs-lookup"><span data-stu-id="08d95-113">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="08d95-114">Microsoft Graph er den anbefalede API til administration af kataloger, identiteter og adgang.</span><span class="sxs-lookup"><span data-stu-id="08d95-114">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="08d95-115">Der er dog stadig nogle få mellemrum mellem, hvad der er muligt i Azure AD Graph og Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="08d95-115">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="08d95-116">Gennemgå følgende artikler, som fremhæver de mest opdaterede forskelle, der kan hjælpe dig med dit valg:</span><span class="sxs-lookup"><span data-stu-id="08d95-116">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="08d95-117">Forskelle i ressourcetyper mellem Azure AD Graph og Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="08d95-117">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="08d95-118">Egenskabsforskelle mellem Azure AD Graph og Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="08d95-118">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="08d95-119">Forskelle på metoden mellem Azure AD og Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="08d95-119">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="08d95-120">**API'en, jeg ringer til, fungerer ikke – hvor kan jeg udføre flere test?**</span><span class="sxs-lookup"><span data-stu-id="08d95-120">**The API I am calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="08d95-121">**Microsoft Graph Explorer** – Test Microsoft Graph-API'er i din lejer eller en demolejer, og se også **eksempelforespørgsler** i Microsoft Graph Explorer.</span><span class="sxs-lookup"><span data-stu-id="08d95-121">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="08d95-122">**Min app er for langsom og bliver også begrænser. Hvilke forbedringer kan jeg foretage?**</span><span class="sxs-lookup"><span data-stu-id="08d95-122">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="08d95-123">Afhængigt af scenariet er der en række forskellige muligheder til rådighed for at gøre dit program mere performant, og i nogle tilfælde mindre tilbøjelig til at blive begrænser af tjenesten (når du foretager for mange opkald).</span><span class="sxs-lookup"><span data-stu-id="08d95-123">Depending on your scenario, there are a variety of options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

- [<span data-ttu-id="08d95-124">Bedste fremgangsmåder for Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="08d95-124">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="08d95-125">Batching af anmodninger</span><span class="sxs-lookup"><span data-stu-id="08d95-125">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="08d95-126">Registrer ændringer via deltaforespørgsel</span><span class="sxs-lookup"><span data-stu-id="08d95-126">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="08d95-127">Få besked om ændringer via webhooks</span><span class="sxs-lookup"><span data-stu-id="08d95-127">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="08d95-128">Begrænsningsvejledning</span><span class="sxs-lookup"><span data-stu-id="08d95-128">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="08d95-129">**Hvor kan jeg finde flere oplysninger om fejl og kendte problemer?**</span><span class="sxs-lookup"><span data-stu-id="08d95-129">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="08d95-130">Oplysninger om fejlsvar i Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="08d95-130">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="08d95-131">Kendte problemer med Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="08d95-131">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="08d95-132">**Hvor kan jeg kontrollere status for tjenestens tilgængelighed og forbindelse?**</span><span class="sxs-lookup"><span data-stu-id="08d95-132">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="08d95-133">Tjenestens tilgængelighed og forbindelse til de underliggende tjenester, der kan tilgås via Microsoft Graph, kan påvirke den overordnede tilgængelighed og ydeevne i Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="08d95-133">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="08d95-134">For Azure Active Directory-tjenestetilstand skal du kontrollere status for **Sikkerhed + Identity-tjenester,** der er angivet på [Azure-statussiden.](https://azure.microsoft.com/status/)</span><span class="sxs-lookup"><span data-stu-id="08d95-134">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="08d95-135">For Office-tjenester, der bidrager til Microsoft Graph, skal du kontrollere status for tjenester, der er angivet på [dashboardet for tjenestetilstand i Office.](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="08d95-135">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="08d95-136">Godkendelsesfejl i Microsoft Graph kan skyldes flere forskellige problemer, hvoraf de fleste genererer en 401- eller 403-fejl.</span><span class="sxs-lookup"><span data-stu-id="08d95-136">Microsoft Graph authorization errors can be a result of several different issues, most of which generate a 401 or 403 error.</span></span> <span data-ttu-id="08d95-137">Følgende kan f.eks. alle føre til godkendelsesfejl:</span><span class="sxs-lookup"><span data-stu-id="08d95-137">For example, the following can all lead to authorization errors:</span></span>

- <span data-ttu-id="08d95-138">Forkerte [flows for erhvervelse af adgangstoken](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)</span><span class="sxs-lookup"><span data-stu-id="08d95-138">Incorrect [access token acquisition flows](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)</span></span>
- <span data-ttu-id="08d95-139">Dårligt konfigurerede [rettighedsområder](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span><span class="sxs-lookup"><span data-stu-id="08d95-139">Poorly configured [permission scopes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span></span>
- <span data-ttu-id="08d95-140">Manglende [samtykke](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span><span class="sxs-lookup"><span data-stu-id="08d95-140">Lack of [consent](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span></span>

<span data-ttu-id="08d95-141">\**_Slutdato for support af ADAL (Azure Active Directory Authentication Library) og AAD Graph (Azure AD Graph API)_* _</span><span class="sxs-lookup"><span data-stu-id="08d95-141">\**_End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)_* _</span></span>

<span data-ttu-id="08d95-142">_*Fra d. 30. juni 2020*\* føjer vi ikke længere nye funktioner til ADAL og Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="08d95-142">_\*Starting June 30th, 2020\*\*, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="08d95-143">Vi yder fortsat teknisk support og sikkerhedsopdateringer, men vil ikke længere levere funktionsopdateringer.</span><span class="sxs-lookup"><span data-stu-id="08d95-143">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="08d95-144">**Fra den 30. juni 2022** afslutter vi understøttelsen af ADAL og Azure AD Graph og yder ikke længere teknisk support eller sikkerhedsopdateringer.</span><span class="sxs-lookup"><span data-stu-id="08d95-144">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="08d95-145">Apps, der bruger ADAL på eksisterende OS-versioner, fungerer fortsat efter dette tidspunkt, men får *ikke teknisk support eller sikkerhedsopdateringer.*</span><span class="sxs-lookup"><span data-stu-id="08d95-145">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="08d95-146">Apps, der bruger Azure AD Graph efter dette tidspunkt, modtager muligvis ikke længere svar fra Azure AD Graph-slutpunktet.</span><span class="sxs-lookup"><span data-stu-id="08d95-146">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="08d95-147">**ADAL-overførsel**</span><span class="sxs-lookup"><span data-stu-id="08d95-147">**ADAL Migration**</span></span>

<span data-ttu-id="08d95-148">Vi anbefaler, at du opdaterer [MSAL (Microsoft Authentication Library)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), som har de nyeste funktioner og sikkerhedsopdateringer.</span><span class="sxs-lookup"><span data-stu-id="08d95-148">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="08d95-149">Hvis du bruger Microsoft-apps, skal du vide, at Microsoft er i gang med at overføre sine programmer til MSAL inden slutdatoen for support, hvilket sikrer, at de får glæde af MSAL's løbende sikkerheds- og funktionsforbedringer.</span><span class="sxs-lookup"><span data-stu-id="08d95-149">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="08d95-150">Læs ofte stillede spørgsmål om ADAL</span><span class="sxs-lookup"><span data-stu-id="08d95-150">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="08d95-151">Få mere at vide om at migrere apps pr. platform</span><span class="sxs-lookup"><span data-stu-id="08d95-151">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="08d95-152">Hvis du har brug for hjælp til at forstå, hvilke af dine apps der bruger ADAL, anbefaler vi, at du gennemgår alle dine apps kildekode og, hvis det er relevant, tager kontakt til eventuelle internetudbydere eller appudbydere.</span><span class="sxs-lookup"><span data-stu-id="08d95-152">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="08d95-153">Microsoft-support kan også give dig en liste over alle ikke-Microsoft ADAL-apps i din lejer.</span><span class="sxs-lookup"><span data-stu-id="08d95-153">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="08d95-154">**AAD Graph Migration**</span><span class="sxs-lookup"><span data-stu-id="08d95-154">**AAD Graph Migration**</span></span>

<span data-ttu-id="08d95-155">For programmer, der bruger Azure AD Graph, skal du følge vores vejledning til [at overføre Azure AD Graph-apps til Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)</span><span class="sxs-lookup"><span data-stu-id="08d95-155">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. <span data-ttu-id="08d95-156">[Vores tjekliste til migrering indeholder et startpunkt](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="08d95-156">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span>
2. <span data-ttu-id="08d95-157">Din registreringsportal til Azure-app viser, hvilke programmer der bruger AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="08d95-157">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="08d95-158">Vi anbefaler, at du gennemser kildekoden til alle dine apps og, hvis det er relevant, skal du kontakte alle internetudbydere eller appudbydere.</span><span class="sxs-lookup"><span data-stu-id="08d95-158">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="08d95-159">Microsoft Support kan også give dig en liste over al AAD Graph-brug i din lejer.</span><span class="sxs-lookup"><span data-stu-id="08d95-159">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="08d95-160">Hvis din app skal have adgang til data i Microsoft Graph, skal brugeren eller administratoren give den de rette tilladelser via en samtykkeproces.</span><span class="sxs-lookup"><span data-stu-id="08d95-160">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="08d95-161">[Tilladelsesreferencen for Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) viser de tilladelser, der er knyttet til hvert overordnede sæt af Microsoft Graph-API'er.</span><span class="sxs-lookup"><span data-stu-id="08d95-161">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="08d95-162">Den indeholder også en vejledning til, hvordan du bruger tilladelserne.</span><span class="sxs-lookup"><span data-stu-id="08d95-162">It also provides guidance about how to use the permissions.</span></span>
