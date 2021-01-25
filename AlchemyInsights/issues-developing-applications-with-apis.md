---
title: Problemer med at udvikle programmer med API'er
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
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974379"
---
# <a name="issues-developing-applications-with-apis"></a><span data-ttu-id="ad705-102">Problemer med at udvikle programmer med API'er</span><span class="sxs-lookup"><span data-stu-id="ad705-102">Issues developing applications with APIs</span></span>

<span data-ttu-id="ad705-103">Du kan komme i gang med at bruge Azure Active Directory-graf-API'ET ved at se vejledning til hurtig start til [Azure ad Graph](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) eller få vist den [interaktive referencedokumentation til Azure ad Graph-API](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span><span class="sxs-lookup"><span data-stu-id="ad705-103">To begin using the Azure Active Directory Graph API, see the [Azure AD Graph API quickstart guide](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , or view the [interactive Azure AD Graph API reference documentation](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span></span>

<span data-ttu-id="ad705-104">**Afslutning af understøttelse af Azure Active Directory-godkendelses bibliotek (ADAL) og Azure AD Graph API (AAD-graf)**</span><span class="sxs-lookup"><span data-stu-id="ad705-104">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="ad705-105">**Starter Juni 30th, 2020**, vil vi ikke længere tilføje nye funktioner til ADAL og Azure ad Graph.</span><span class="sxs-lookup"><span data-stu-id="ad705-105">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="ad705-106">Vi vil fortsat yde teknisk support og sikkerhedsopdateringer, men vil ikke længere tilbyde FUNKTIONSOPDATERINGER.</span><span class="sxs-lookup"><span data-stu-id="ad705-106">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="ad705-107">**Fra og med juni 30th, 2022**, vi slutter support til ADAL og Azure ad Graph og vil ikke længere yde teknisk support eller sikkerhedsopdateringer.</span><span class="sxs-lookup"><span data-stu-id="ad705-107">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="ad705-108">Apps, der bruger ADAL på eksisterende OS-versioner, vil fortsat fungere efter dette tidspunkt, men de får ikke teknisk support eller sikkerhedsopdateringer.</span><span class="sxs-lookup"><span data-stu-id="ad705-108">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

<span data-ttu-id="ad705-109">Apps, der bruger Azure AD Graph efter dette tidspunkt, kan muligvis ikke længere modtage svar fra Azure AD Graph-slutpunktet.</span><span class="sxs-lookup"><span data-stu-id="ad705-109">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="ad705-110">**ADAL-overførsel**</span><span class="sxs-lookup"><span data-stu-id="ad705-110">**ADAL Migration**</span></span>

<span data-ttu-id="ad705-111">Vi anbefaler, at du opdaterer til [Microsoft-godkendelses bibliotek (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), som har de nyeste funktioner og sikkerhedsopdateringer.</span><span class="sxs-lookup"><span data-stu-id="ad705-111">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="ad705-112">Hvis du bruger Microsoft-apps, skal du vide, at Microsoft er i gang med at overføre sine programmer til MSAL ved hjælp af deadline for sidste support, så de kan drage fordel af MSAL de vedvarende sikkerheds-og funktionsforbedringer.</span><span class="sxs-lookup"><span data-stu-id="ad705-112">If you're using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="ad705-113">[Læs ADAL ofte stillede spørgsmål](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="ad705-113">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="ad705-114">[Få mere at vide om, hvordan du kan overføre apps på et enkelt platforms grundlag](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="ad705-114">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="ad705-115">Hvis du har brug for hjælp til at forstå, hvilke af dine apps der bruger ADAL, anbefaler vi, at du gennemgår alle dine apps-kildekode, og hvis det er relevant, kan du få adgang til alle ISV'er-eller app-udbydere.</span><span class="sxs-lookup"><span data-stu-id="ad705-115">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="ad705-116">Microsoft Support kan også give dig en liste over alle ikke-Microsoft-ADAL-apps i din lejer.</span><span class="sxs-lookup"><span data-stu-id="ad705-116">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="ad705-117">**AAD-diagram overførsel**</span><span class="sxs-lookup"><span data-stu-id="ad705-117">**AAD Graph Migration**</span></span>

<span data-ttu-id="ad705-118">For programmer, der bruger Azure AD Graph, skal du følge vores vejledning til at overføre [Azure ad Graph-apps til Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="ad705-118">For applications that are using Azure AD Graph, follow our guidance to migrate [Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span></span>

1. <span data-ttu-id="ad705-119">[Vores overflytnings checkliste giver et](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)introduktions point.</span><span class="sxs-lookup"><span data-stu-id="ad705-119">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
1. <span data-ttu-id="ad705-120">Din Azure-app-registrerings Portal viser, hvilke programmer der bruger AAD-grafer.</span><span class="sxs-lookup"><span data-stu-id="ad705-120">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="ad705-121">Vi anbefaler, at du gennemgår alle din apps-kildekode, og hvis det er relevant, så du kan få adgang til alle ISV'er-eller app-udbydere.</span><span class="sxs-lookup"><span data-stu-id="ad705-121">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="ad705-122">Microsoft Support kan også give dig en liste over alle AAD-diagram brug i din lejer.</span><span class="sxs-lookup"><span data-stu-id="ad705-122">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
1. <span data-ttu-id="ad705-123">Hvis din app skal have adgang til data i Microsoft Graph, skal brugeren eller administratoren give den de rette tilladelser via en tilladelses proces.</span><span class="sxs-lookup"><span data-stu-id="ad705-123">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="ad705-124">[Microsoft Graph-tilladelses referencen](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) viser de tilladelser, der er knyttet til hvert omfattende sæt Microsoft Graph-API'er.</span><span class="sxs-lookup"><span data-stu-id="ad705-124">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="ad705-125">Den indeholder også en vejledning til, hvordan du brugertilladelserne.</span><span class="sxs-lookup"><span data-stu-id="ad705-125">It also provides guidance about how to use the permissions.</span></span>
