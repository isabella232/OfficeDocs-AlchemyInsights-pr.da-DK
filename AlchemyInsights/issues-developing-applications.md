---
title: Problemer med at udvikle programmer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974306"
---
# <a name="issues-developing-applications"></a><span data-ttu-id="d7f86-102">Problemer med at udvikle programmer</span><span class="sxs-lookup"><span data-stu-id="d7f86-102">Issues developing applications</span></span>

<span data-ttu-id="d7f86-103">Hvis du vil foretage fejlfinding af de mest almindelige problemer ved oprettelse af Azure Active Directory (AD)-apps, skal du se følgende artikler:</span><span class="sxs-lookup"><span data-stu-id="d7f86-103">To troubleshoot the most common problems when building Azure Active Directory (AD) apps, see the following articles:</span></span>

- [<span data-ttu-id="d7f86-104">Jeg kan se problemer med at logge på programmer ved hjælp af Chrome-browser</span><span class="sxs-lookup"><span data-stu-id="d7f86-104">I am seeing trouble signing in to application(s) using Chrome browser only</span></span>](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [<span data-ttu-id="d7f86-105">Jeg ved ikke, hvordan du ændrer standarderne for token-levetid for mit program</span><span class="sxs-lookup"><span data-stu-id="d7f86-105">I don't know how to change the token lifetime defaults for my application</span></span>](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [<span data-ttu-id="d7f86-106">Jeg er usikker på, hvordan program samtykke fungerer</span><span class="sxs-lookup"><span data-stu-id="d7f86-106">I am confused about how application consent works</span></span>](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [<span data-ttu-id="d7f86-107">Jeg ved ikke, hvordan jeg giver tilladelse til mit program</span><span class="sxs-lookup"><span data-stu-id="d7f86-107">I don't know how to grant permissions to my application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [<span data-ttu-id="d7f86-108">Jeg forstår ikke forskellen mellem delegerede og program tilladelser</span><span class="sxs-lookup"><span data-stu-id="d7f86-108">I don't understand the difference between delegated and application permissions</span></span>](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

<span data-ttu-id="d7f86-109">\***Slutningen af understøttelse af Azure Active Directory-godkendelses bibliotek (ADAL) og Azure ad Graph API (Aad-graf)** _</span><span class="sxs-lookup"><span data-stu-id="d7f86-109">\***End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)** _</span></span>

- <span data-ttu-id="d7f86-110">Fra juni 30th, 2020, vil vi ikke længere tilføje nye funktioner til Azure Active Directory-godkendelses bibliotek (ADAL) og Azure AD graf API (AAD-graf).</span><span class="sxs-lookup"><span data-stu-id="d7f86-110">Starting June 30th, 2020, we will no longer add any new features to Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph).</span></span> <span data-ttu-id="d7f86-111">Vi vil fortsat yde teknisk support og sikkerhedsopdateringer, men vil ikke længere tilbyde FUNKTIONSOPDATERINGER.</span><span class="sxs-lookup"><span data-stu-id="d7f86-111">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

- <span data-ttu-id="d7f86-112">Fra juni 30th, 2022, vi afslutter support til ADAL og AAD-grafen og vil ikke længere yde teknisk support eller sikkerhedsopdateringer.</span><span class="sxs-lookup"><span data-stu-id="d7f86-112">Starting June 30th, 2022, we will end support for ADAL and AAD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="d7f86-113">Som følge af denne betingelse gælder følgende:</span><span class="sxs-lookup"><span data-stu-id="d7f86-113">As a result of this condition, the following are the implications:</span></span>

    - <span data-ttu-id="d7f86-114">Apps, der bruger ADAL på eksisterende OS-versioner, vil fortsat fungere efter dette tidspunkt, men de får ikke teknisk support eller sikkerhedsopdateringer.</span><span class="sxs-lookup"><span data-stu-id="d7f86-114">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

    - <span data-ttu-id="d7f86-115">Apps, der bruger AAD Graph efter dette tidspunkt, kan muligvis ikke længere modtage svar fra det AAD-diagram slutpunkt</span><span class="sxs-lookup"><span data-stu-id="d7f86-115">Apps using AAD Graph after this time may no longer receive responses from the AAD Graph endpoint</span></span>

<span data-ttu-id="d7f86-116">_ *ADAL-overførsel*\*</span><span class="sxs-lookup"><span data-stu-id="d7f86-116">_ *ADAL Migration*\*</span></span>

<span data-ttu-id="d7f86-117">Hvis du bruger Microsoft-apps, anbefaler vi, at du opdaterer til Microsoft-godkendelses bibliotek (MSAL), som har de nyeste funktioner og sikkerhedsopdateringer.</span><span class="sxs-lookup"><span data-stu-id="d7f86-117">If you're using Microsoft apps, we recommend updating to the Microsoft Authentication Library (MSAL), which has the latest features and security updates.</span></span> <span data-ttu-id="d7f86-118">Denne anbefaling er i forbindelse med Microsoft, der starter processen med at overføre sine apps til MSAL ved hjælp af deadline for support.</span><span class="sxs-lookup"><span data-stu-id="d7f86-118">This recommendation is in the context of Microsoft initiating the process of migrating its apps to MSAL by the end-of-support deadline.</span></span> 

<span data-ttu-id="d7f86-119">Overførslen af Microsofts apps til MSAL sikrer, at apps nyder godt af de vedvarende sikkerheds-og funktionsforbedringer for MSAL.</span><span class="sxs-lookup"><span data-stu-id="d7f86-119">The migration by Microsoft of its apps to MSAL ensures that the apps benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="d7f86-120">Læs ADAL ofte stillede spørgsmål</span><span class="sxs-lookup"><span data-stu-id="d7f86-120">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [<span data-ttu-id="d7f86-121">Få mere at vide om, hvordan du kan overføre apps på et enkelt platforms grundlag</span><span class="sxs-lookup"><span data-stu-id="d7f86-121">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. <span data-ttu-id="d7f86-122">Hvis du har brug for hjælp til at forstå, hvilke af dine apps der bruger ADAL, anbefaler vi, at du gennemgår alle dine apps-kildekode, og hvis det er relevant, at få adgang til uafhængige softwareleverandører eller app-udbydere.</span><span class="sxs-lookup"><span data-stu-id="d7f86-122">If you need help in understanding which of your apps use ADAL, we recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="d7f86-123">Microsoft Support kan også give dig en liste over alle ikke-Microsoft-ADAL-apps i din lejer.</span><span class="sxs-lookup"><span data-stu-id="d7f86-123">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="d7f86-124">**AAD-diagram overførsel**</span><span class="sxs-lookup"><span data-stu-id="d7f86-124">**AAD Graph Migration**</span></span>

<span data-ttu-id="d7f86-125">For programmer, der bruger AAD-graf, skal du følge vores vejledning til at overføre AAD-apps til Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="d7f86-125">For applications that are using AAD Graph, follow our guidance to migrate AAD Graph apps to Microsoft Graph:</span></span>

1. <span data-ttu-id="d7f86-126">[Vores overflytnings checkliste giver et](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)introduktions point.</span><span class="sxs-lookup"><span data-stu-id="d7f86-126">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
2. <span data-ttu-id="d7f86-127">Din Azure-app-registrerings Portal viser, hvilke programmer der bruger AAD-grafer.</span><span class="sxs-lookup"><span data-stu-id="d7f86-127">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="d7f86-128">Vi anbefaler, at du gennemgår alle dine apps-kildekoder, og hvis det er relevant, at få adgang til uafhængige softwareleverandører eller app-udbydere.</span><span class="sxs-lookup"><span data-stu-id="d7f86-128">We recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="d7f86-129">Microsoft Support kan også give dig oplysninger om AAD-diagram brug i din lejer.</span><span class="sxs-lookup"><span data-stu-id="d7f86-129">Microsoft support can also provide you information on AAD Graph usage in your tenant.</span></span>







