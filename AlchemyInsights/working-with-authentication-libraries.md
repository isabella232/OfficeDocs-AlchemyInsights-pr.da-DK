---
title: Arbejde med godkendelsesbiblioteker
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035288"
---
# <a name="working-with-authentication-libraries"></a><span data-ttu-id="5e2a0-102">Arbejde med godkendelsesbiblioteker</span><span class="sxs-lookup"><span data-stu-id="5e2a0-102">Working with Authentication Libraries</span></span>

<span data-ttu-id="5e2a0-103">Du kan løse problemet med Microsoft-godkendelsesbiblioteket (MSAL) ved at udføre følgende anbefalede trin:</span><span class="sxs-lookup"><span data-stu-id="5e2a0-103">To resolve Microsoft Authentication Library (MSAL) issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="5e2a0-104">**Arbejde med MSAL:** [Godkendelsesbiblioteker for Microsoft-identitetsplatformen](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) – Denne artikel viser understøttelse af Microsoft-godkendelsesbiblioteket for flere programtyper.</span><span class="sxs-lookup"><span data-stu-id="5e2a0-104">**Working with MSAL**: [Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - This article shows Microsoft Authentication Library support for several application types.</span></span> <span data-ttu-id="5e2a0-105">Den indeholder links til bibliotekskildekode; hvor du kan hente pakken til din apps projekt; og om biblioteket understøtter brugeradgang (godkendelse), adgang til beskyttede web-API'er (godkendelse) eller begge dele.</span><span class="sxs-lookup"><span data-stu-id="5e2a0-105">It includes links to library source code; where to get the package for your app's project; and whether the library supports user sign-in (authentication), access to protected web APIs (authorization), or both.</span></span>

2. <span data-ttu-id="5e2a0-106">**Fejlfinding af godkendelse:** MSAL understøtter flere godkendelsesflows til brug i forskellige programscenarier.</span><span class="sxs-lookup"><span data-stu-id="5e2a0-106">**Troubleshoot Authentication**: The MSAL supports several authentication flows for use in different application scenarios.</span></span> <span data-ttu-id="5e2a0-107">Afhængigt af hvordan dit klientprogram er opbygget, kan MSAL bruge en eller flere af de godkendelsesflows, der understøttes af Microsoft-identitetsplatformen.</span><span class="sxs-lookup"><span data-stu-id="5e2a0-107">Depending on how your client application is built, the MSAL can use one or more of the authentication flows supported by the Microsoft identity platform.</span></span> <span data-ttu-id="5e2a0-108">Disse flows kan give flere typer tokens og godkendelseskoder og kræve forskellige tokens for at få dem til at fungere.</span><span class="sxs-lookup"><span data-stu-id="5e2a0-108">These flows can produce several types of tokens and authorization codes, and require different tokens to make them work.</span></span>

3. <span data-ttu-id="5e2a0-109">**Adgangstokens:** [Adgangstokens fra Microsoft-identitetsplatformen](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) – Få mere at vide om, hvordan din API kan validere og bruge krav i et adgangstoken.</span><span class="sxs-lookup"><span data-stu-id="5e2a0-109">**Access Tokens**: [Microsoft identity platform access tokens](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Learn how your API can validate and use the claims inside an access token.</span></span> <span data-ttu-id="5e2a0-110">Al dokumentation i denne artikel, undtagen hvor den er angivet, gælder kun for tokens, der er udstedt for API'er, du har registreret.</span><span class="sxs-lookup"><span data-stu-id="5e2a0-110">All documentation in this article, except where noted, applies only to tokens issued for APIs you've registered.</span></span> <span data-ttu-id="5e2a0-111">Den gælder ikke for tokens, der er udstedt for Microsoft-ejet API'er, og disse tokens kan heller ikke bruges til at validere, hvordan Microsoft-identitetsplatformen udsteder tokens for en API, du opretter.</span><span class="sxs-lookup"><span data-stu-id="5e2a0-111">It does not apply to tokens issued for Microsoft-owned APIs, nor can those tokens be used to validate how the Microsoft identity platform will issue tokens for an API you create.</span></span>

<span data-ttu-id="5e2a0-112">**Ophør af understøttelse af Azure Active Directory Authentication Library (ADAL)**</span><span class="sxs-lookup"><span data-stu-id="5e2a0-112">**End of support for Azure Active Directory Authentication Library (ADAL)**</span></span>

- <span data-ttu-id="5e2a0-113">**Fra den 30. juni 2020** tilføjer vi ikke længere nye funktioner til ADAL og Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="5e2a0-113">**Starting June 30th, 2020,** we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="5e2a0-114">Vi yder fortsat teknisk support og sikkerhedsopdateringer, men vil ikke længere levere funktionsopdateringer.</span><span class="sxs-lookup"><span data-stu-id="5e2a0-114">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
- <span data-ttu-id="5e2a0-115">**Fra d. 30. juni 2022** afslutter vi understøttelsen af ADAL og Azure AD Graph og yder ikke længere teknisk support eller sikkerhedsopdateringer.</span><span class="sxs-lookup"><span data-stu-id="5e2a0-115">**Starting June 30th, 2022,** we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>
- <span data-ttu-id="5e2a0-116">Apps, der bruger ADAL på eksisterende OS-versioner, fungerer fortsat efter dette tidspunkt, men får *ikke teknisk support eller sikkerhedsopdateringer.*</span><span class="sxs-lookup"><span data-stu-id="5e2a0-116">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>
- <span data-ttu-id="5e2a0-117">Apps, der bruger Azure AD Graph efter dette tidspunkt, modtager muligvis ikke længere svar fra Azure AD Graph-slutpunktet.</span><span class="sxs-lookup"><span data-stu-id="5e2a0-117">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="5e2a0-118">**ADAL-overførsel**</span><span class="sxs-lookup"><span data-stu-id="5e2a0-118">**ADAL Migration**</span></span>

- <span data-ttu-id="5e2a0-119">Vi anbefaler at opdatere til MSAL, som har de nyeste funktioner og sikkerhedsopdateringer.</span><span class="sxs-lookup"><span data-stu-id="5e2a0-119">We recommend updating to the MSAL, which has the latest features and security updates.</span></span>
- <span data-ttu-id="5e2a0-120">Hvis du bruger Microsoft-apps, skal du vide, at Microsoft er i gang med at overføre sine apps til MSAL inden slutdatoen for support, hvilket sikrer, at de får glæde af MSAL's løbende sikkerheds- og funktionsforbedringer.</span><span class="sxs-lookup"><span data-stu-id="5e2a0-120">If you're using Microsoft apps, know that Microsoft is in the process of migrating its apps to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="5e2a0-121">[Læs ofte stillede spørgsmål om ADAL.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)</span><span class="sxs-lookup"><span data-stu-id="5e2a0-121">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
2. <span data-ttu-id="5e2a0-122">[Få mere at vide om, hvordan du overfører apps på pr. platform.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance)</span><span class="sxs-lookup"><span data-stu-id="5e2a0-122">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span></span>
3. <span data-ttu-id="5e2a0-123">Hvis du efter at have læst vejledningen til din apps platform har yderligere spørgsmål, kan du skrive et opslag på [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) med mærket [azure-ad-adal-deprecation] eller åbne et problem i bibliotekets GitHub-lager.</span><span class="sxs-lookup"><span data-stu-id="5e2a0-123">If, after reading the guide for your app's platform, you have additional questions, you can post on [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) with the tag [azure-ad-adal-deprecation] or open an issue in library's GitHub repository.</span></span> <span data-ttu-id="5e2a0-124">Se afsnittet Sprog og rammer i **MSAL-oversigtsartikel** for links til hvert [biblioteks](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) repo.</span><span class="sxs-lookup"><span data-stu-id="5e2a0-124">See the [Languages and frameworks](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) section of the **MSAL overview** article for links to each library's repo.</span></span>
4. <span data-ttu-id="5e2a0-125">**Hvis du har brug for hjælp til at forstå, hvilke af** dine apps der bruger ADAL, anbefaler vi, at du gennemgår alle dine apps kildekode.</span><span class="sxs-lookup"><span data-stu-id="5e2a0-125">**If you need help understanding which of your apps use ADAL**, we recommend you review all of your apps' source code.</span></span> <span data-ttu-id="5e2a0-126">Hvis det er relevant, skal du kontakte eventuelle uafhængige softwareleverandører eller appudbydere.</span><span class="sxs-lookup"><span data-stu-id="5e2a0-126">If applicable, reach out to any Independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="5e2a0-127">Microsoft-support kan også give dig en liste over alle ikke-Microsoft ADAL-apps i din lejer.</span><span class="sxs-lookup"><span data-stu-id="5e2a0-127">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>







