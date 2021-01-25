---
title: Forespørgsel til Microsoft Graph API
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
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974283"
---
# <a name="querying-the-microsoft-graph-api"></a><span data-ttu-id="b9198-102">Forespørgsel til Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="b9198-102">Querying the Microsoft Graph API</span></span>

<span data-ttu-id="b9198-103">Dette emne gælder muligvis også for udviklere, der stadig bruger Azure AD Graph API.</span><span class="sxs-lookup"><span data-stu-id="b9198-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="b9198-104">Det anbefales dog på det **kraftigste** , at du bruger Microsoft Graph til alle scenarier for katalog, identitet og adgangsstyring.</span><span class="sxs-lookup"><span data-stu-id="b9198-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="b9198-105">**Godkendelses-eller godkendelsesproblemer**</span><span class="sxs-lookup"><span data-stu-id="b9198-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="b9198-106">Hvis din app **ikke kan hente tokens** til at ringe til Microsoft Graph, skal du vælge **problem med at få en Access-token (Authentication)** Microsoft Graph-kategori for at få mere specifik hjælp og support til dette emne.</span><span class="sxs-lookup"><span data-stu-id="b9198-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="b9198-107">Hvis din app **modtager 401-eller 403-godkendelsesfejl** , når du ringer til Microsoft Graph, skal du vælge Microsoft Graph-API **-kategorien få adgang nægtet (godkendelse)** til at få mere specifik hjælp og support i dette emne.</span><span class="sxs-lookup"><span data-stu-id="b9198-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="b9198-108">**Jeg vil bruge Microsoft Graph, men ikke sikker på, hvor du skal starte**</span><span class="sxs-lookup"><span data-stu-id="b9198-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

<span data-ttu-id="b9198-109">Du kan få mere at vide om Microsoft Graph i:</span><span class="sxs-lookup"><span data-stu-id="b9198-109">To learn more about Microsoft Graph, see:</span></span>

- [<span data-ttu-id="b9198-110">Oversigt over Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b9198-110">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="b9198-111">Oversigt over identitets-og adgangsstyring i Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b9198-111">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="b9198-112">Introduktion til oprettelse af Microsoft Graph-apps</span><span class="sxs-lookup"><span data-stu-id="b9198-112">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="b9198-113">**Microsoft Graph Explorer** -test Microsoft Graph-API'er i din lejer eller en demo lejer</span><span class="sxs-lookup"><span data-stu-id="b9198-113">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="b9198-114">**Jeg vil bruge Microsoft Graph, men det understøtter ikke det v 1.0-katalog-API'er, jeg har brug for?**</span><span class="sxs-lookup"><span data-stu-id="b9198-114">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="b9198-115">Microsoft Graph er den anbefalede API til katalog, identitet og adgangs administration.</span><span class="sxs-lookup"><span data-stu-id="b9198-115">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="b9198-116">Der er dog stadig nogle mellemrum mellem det, der er muligt i Azure AD Graph og Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b9198-116">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="b9198-117">Gennemgå følgende artikler, som fremhæver de mest opdaterede forskelle for at hjælpe dig med dit valg:</span><span class="sxs-lookup"><span data-stu-id="b9198-117">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="b9198-118">Forskelle mellem ressourcetyperne i Azure AD Graph og Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b9198-118">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="b9198-119">Forskelle mellem egenskaber mellem Azure AD Graph og Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b9198-119">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="b9198-120">Metode forskelle mellem Azure AD og Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b9198-120">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="b9198-121">**Når jeg opretter en forespørgsel i *bruger* objektet, mangler der mange egenskaber**</span><span class="sxs-lookup"><span data-stu-id="b9198-121">**When I query the *user* object, many of its properties are missing**</span></span>

<span data-ttu-id="b9198-122">`GET https://graph.microsoft.com/v1.0/users` returnerer kun 11-egenskaber, da Microsoft Graph automatisk vælger et standardsæt af *bruger* egenskaber, der skal returneres.</span><span class="sxs-lookup"><span data-stu-id="b9198-122">`GET https://graph.microsoft.com/v1.0/users` only returns 11 properties, as Microsoft Graph auto-selects a default set of *user* properties to return.</span></span> <span data-ttu-id="b9198-123">Hvis du har brug for andre *bruger* egenskaber, kan du bruge $Select til at vælge de egenskaber, som programmet skal bruge.</span><span class="sxs-lookup"><span data-stu-id="b9198-123">If you need other *user* properties, use $select to pick the properties your application needs.</span></span> <span data-ttu-id="b9198-124">Prøv det i **Microsoft Graph Explorer** først.</span><span class="sxs-lookup"><span data-stu-id="b9198-124">Try it out in **Microsoft Graph Explorer** first.</span></span>

<span data-ttu-id="b9198-125">**Nogle bruger egenskabsværdier er *Null* , også selvom jeg ved, at de er angivet**</span><span class="sxs-lookup"><span data-stu-id="b9198-125">**Some user property values are *null* even though I know they are set**</span></span>

<span data-ttu-id="b9198-126">Den mest sandsynlige forklaring er, at programmet har fået tildelt *brugeren. ReadBasic. alle* tilladelser.</span><span class="sxs-lookup"><span data-stu-id="b9198-126">The most likely explanation is that the application had been granted the *User.ReadBasic.All* permission.</span></span> <span data-ttu-id="b9198-127">Dette gør det muligt for programmet at læse et begrænset sæt af bruger egenskaber, der returnerer alle andre egenskaber som null, selvom de tidligere er angivet.</span><span class="sxs-lookup"><span data-stu-id="b9198-127">This allows the application to read a limited set of user properties, returning all other properties as null even if they have been previously set.</span></span> <span data-ttu-id="b9198-128">Prøv at tildele program *brugeren. Læs. alle* tilladelser i stedet.</span><span class="sxs-lookup"><span data-stu-id="b9198-128">Try granting the application *User.Read.All* permission instead.</span></span>

<span data-ttu-id="b9198-129">Du kan finde flere oplysninger i [Microsoft Graph-brugertilladelser](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span><span class="sxs-lookup"><span data-stu-id="b9198-129">For more information, see [Microsoft Graph user permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span></span>

<span data-ttu-id="b9198-130">**Jeg har problemer med at bruge OData-forespørgselsparametre til at filtrere data i mine anmodninger**</span><span class="sxs-lookup"><span data-stu-id="b9198-130">**I'm having trouble using OData query parameters to filter data in my requests**</span></span>

<span data-ttu-id="b9198-131">Selvom Microsoft Graph understøtter en lang række OData-forespørgselsparametre, understøttes mange af disse parametre ikke fuldt ud af katalogtjenester (ressourcer, der nedarves fra *directoryObject*) i Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b9198-131">While Microsoft Graph supports a wide range of the OData query parameters, many of those parameters are not fully supported by directory services (resources that inherit from *directoryObject*) in Microsoft Graph.</span></span> <span data-ttu-id="b9198-132">De samme begrænsninger, der blev vist i Azure AD Graph, bevares i Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="b9198-132">The same limitations that were present in Azure AD Graph persist for the most part in Microsoft Graph:</span></span>

1. <span data-ttu-id="b9198-133">**Understøttes ikke**: $count, $search og $filter på *Null* eller *NOT NULL* -værdier</span><span class="sxs-lookup"><span data-stu-id="b9198-133">**Not supported**: $count, $search, and $filter on *null* or *not null* values</span></span>
2. <span data-ttu-id="b9198-134">**Understøttes ikke**: $filter på visse egenskaber (Se ressource emner, der indeholder de egenskaber, der kan filtreres)</span><span class="sxs-lookup"><span data-stu-id="b9198-134">**Not supported**: $filter on certain properties (see resource topics on which properties are filterable)</span></span>
3. <span data-ttu-id="b9198-135">**Understøttes ikke**: paging, filtrering og sortering på samme tid</span><span class="sxs-lookup"><span data-stu-id="b9198-135">**Not supported**: paging, filtering, and sorting at the same time</span></span>
4. <span data-ttu-id="b9198-136">**Understøttes ikke**: filtrering af en relation.</span><span class="sxs-lookup"><span data-stu-id="b9198-136">**Not supported**: filtering on a relationship.</span></span> <span data-ttu-id="b9198-137">For eksempel – Find alle medlemmer af gruppen teknikere, der er i Storbritannien.</span><span class="sxs-lookup"><span data-stu-id="b9198-137">For example - find all members of the engineering group that are in the UK.</span></span>
5. <span data-ttu-id="b9198-138">**Delvis support**: $OrderBy *bruger* (kun DisplayName og userPrincipalName) og *gruppe*</span><span class="sxs-lookup"><span data-stu-id="b9198-138">**Partial support**: $orderby on *user* (displayName and userPrincipalName only) and *group*</span></span>
6. <span data-ttu-id="b9198-139">**Delvis understøttelse**: $filter (understøtter kun *EQ*-, *StartsWith*- *eller* *og begr* ænset *en*) understøttelse, $Expand (udvidelse af relationerne mellem et enkelt objekt returnerer alle relationer, men udvidelse af en samling af objektrelationer er begrænset)</span><span class="sxs-lookup"><span data-stu-id="b9198-139">**Partial support**: $filter (supports only *eq*, *startswith*, *or*, *and*, and limited *any*) support, $expand (expanding a single object's relationships returns all relationships, but expanding a collection of objects' relationships is limited)</span></span>

<span data-ttu-id="b9198-140">Hvis du vil have mere at vide, skal du se [tilpasse svar med forespørgselsparametre](https://docs.microsoft.com/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b9198-140">For more information, see [Customize responses with query parameters](https://docs.microsoft.com/graph/query-parameters).</span></span>

<span data-ttu-id="b9198-141">**API'EN, jeg ringer til, fungerer ikke – hvor kan jeg foretage flere tests?**</span><span class="sxs-lookup"><span data-stu-id="b9198-141">**The API I'm calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="b9198-142">**Microsoft Graph Explorer** -test Microsoft Graph-API'er i din lejer eller en demo lejer, og se også **eksempel forespørgslerne** i Microsoft Graph Explorer.</span><span class="sxs-lookup"><span data-stu-id="b9198-142">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="b9198-143">**Når jeg opretter en forespørgsel efter data, ser det ud til, at jeg får et ufuldstændigt datasæt tilbage**</span><span class="sxs-lookup"><span data-stu-id="b9198-143">**When I query for data it seems like I get an incomplete data set back**</span></span>

<span data-ttu-id="b9198-144">Hvis du forespørger en samling (som *brugere*), bruger Microsoft Graph serverside begrænsninger, så resultaterne altid returneres med en standardsidestørrelse.</span><span class="sxs-lookup"><span data-stu-id="b9198-144">If you are querying a collection (like *users*), Microsoft Graph uses server-side page limits so results are always returned with a default page-size.</span></span> <span data-ttu-id="b9198-145">Din app bør altid forvente at side gennem samlinger, der returneres fra tjenesten.</span><span class="sxs-lookup"><span data-stu-id="b9198-145">Your app should always expect to page through collections returned from the service.</span></span>

<span data-ttu-id="b9198-146">Du kan finde flere oplysninger under:</span><span class="sxs-lookup"><span data-stu-id="b9198-146">For more information, see:</span></span>

- [<span data-ttu-id="b9198-147">Bedste fremgangsmåder for Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b9198-147">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="b9198-148">Side om at overskrive Microsoft Graph-data i din app</span><span class="sxs-lookup"><span data-stu-id="b9198-148">Paging Microsoft Graph data in your app</span></span>](https://docs.microsoft.com/graph/paging)

<span data-ttu-id="b9198-149">**Min app er for langsom og får også begrænset det. Hvilke forbedringer kan jeg lave?**</span><span class="sxs-lookup"><span data-stu-id="b9198-149">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="b9198-150">Afhængigt af dit scenarie er der en række forskellige muligheder for din rådighed til at gøre dit programmere drifts nært, og i nogle tilfælde, hvor du kan blive begrænset af tjenesten (når du foretager for mange opkald).</span><span class="sxs-lookup"><span data-stu-id="b9198-150">Depending on your scenario, there are a variety of different options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

<span data-ttu-id="b9198-151">Du kan få mere at vide under:</span><span class="sxs-lookup"><span data-stu-id="b9198-151">To learn more, see:</span></span>

- [<span data-ttu-id="b9198-152">Bedste fremgangsmåder for Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b9198-152">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="b9198-153">Anmodninger om batch</span><span class="sxs-lookup"><span data-stu-id="b9198-153">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="b9198-154">Registrer ændringer via en Delta forespørgsel</span><span class="sxs-lookup"><span data-stu-id="b9198-154">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="b9198-155">Få besked om ændringer via webhooks</span><span class="sxs-lookup"><span data-stu-id="b9198-155">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="b9198-156">Begrænset vejledning</span><span class="sxs-lookup"><span data-stu-id="b9198-156">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="b9198-157">**Hvor kan jeg finde flere oplysninger om fejl og kendte problemer?**</span><span class="sxs-lookup"><span data-stu-id="b9198-157">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="b9198-158">Oplysninger om fejlsvar i Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b9198-158">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="b9198-159">Kendte problemer med Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b9198-159">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="b9198-160">**Hvor kan jeg kontrollere status for tjenestens tilgængelighed og forbindelse?**</span><span class="sxs-lookup"><span data-stu-id="b9198-160">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="b9198-161">Tjenestens tilgængelighed og forbindelse mellem de underliggende tjenester, der kan åbnes gennem Microsoft Graph, kan påvirke den overordnede tilgængelighed og ydeevne i Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b9198-161">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="b9198-162">For Azure Active Directory-tjenestetilstand skal du kontrollere status for **sikkerheds + identitets** tjenester, der er angivet på [siden Azure-status](https://azure.microsoft.com/status/).</span><span class="sxs-lookup"><span data-stu-id="b9198-162">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="b9198-163">For Office-tjenester, der bidrager til Microsoft Graph, skal du kontrollere status for tjenester, der er angivet i [dashboardet til Office-tjenestetilstand](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="b9198-163">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
