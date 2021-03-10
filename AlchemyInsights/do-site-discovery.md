---
title: Do site discovery
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692937"
---
# <a name="do-site-discovery"></a><span data-ttu-id="746fa-102">Do site discovery</span><span class="sxs-lookup"><span data-stu-id="746fa-102">Do site discovery</span></span>

<span data-ttu-id="746fa-103">Hvis din organisation stadig bruger ældre webprogrammer og planer om at bruge Internet Explorer-tilstand (hvilket de fleste kunder gør), skal du gøre noget yderligere opdagelse af webstedet.</span><span class="sxs-lookup"><span data-stu-id="746fa-103">If your organization still uses legacy web applications and plans to use Internet Explorer mode (which most customers do), then you should do some additional site discovery.</span></span>

<span data-ttu-id="746fa-104">**Du har allerede installeret en ældre version af Microsoft Edge**</span><span class="sxs-lookup"><span data-stu-id="746fa-104">**You've already deployed an older version of Microsoft Edge**</span></span>

<span data-ttu-id="746fa-105">Hvis du allerede har konfigureret din enterprise-webstedsliste til at fungere for den ældre version af Microsoft Edge, er din webstedsregistrering næsten færdig.</span><span class="sxs-lookup"><span data-stu-id="746fa-105">If you've already configured your Enterprise Site List to work for the legacy version of Microsoft Edge, then your site discovery is almost done.</span></span> <span data-ttu-id="746fa-106">Den eneste, du muligvis skal gøre, er at tilføje neutrale websteder.</span><span class="sxs-lookup"><span data-stu-id="746fa-106">The one thing you might need to do is add neutral sites.</span></span>

<span data-ttu-id="746fa-107">Neutrale websteder er typisk websteder, der leverer enkelt-logon (SSO).</span><span class="sxs-lookup"><span data-stu-id="746fa-107">Neutral sites are typically sites that provide single sign-on (SSO).</span></span> <span data-ttu-id="746fa-108">Hvis du går til et neutralt websted fra Microsoft Edge, vil du forblive i Microsoft Edge for at godkende.</span><span class="sxs-lookup"><span data-stu-id="746fa-108">If you go to a neutral site from Microsoft Edge, then you want to stay in Microsoft Edge to authenticate.</span></span> <span data-ttu-id="746fa-109">Hvis du går til et neutralt websted i Internet Explorer-tilstand, vil du forblive i Internet Explorer-tilstand for at godkende.</span><span class="sxs-lookup"><span data-stu-id="746fa-109">If you go to a neutral site in Internet Explorer mode, then you want to stay in Internet Explorer mode to authenticate.</span></span>

<span data-ttu-id="746fa-110">Identificer eventuelle SSO-websteder eller andre neutrale websteder, du bruger, og føj dem til din enterprise-webstedsliste.</span><span class="sxs-lookup"><span data-stu-id="746fa-110">Identify any SSO or other neutral sites that you use and add these to your Enterprise Site List.</span></span>

<span data-ttu-id="746fa-111">**Internet Explorer er din standardbrowser**</span><span class="sxs-lookup"><span data-stu-id="746fa-111">**Internet Explorer is your default browser**</span></span>

<span data-ttu-id="746fa-112">Hvis du kun bruger Internet Explorer nu, ved du muligvis ikke, hvilke websteder der har opgraderet til moderne webstandarder, og hvilke der stadig kræver Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="746fa-112">If you're only using Internet Explorer now, you might not know which sites have upgraded to modern web standards and which still require Internet Explorer.</span></span> <span data-ttu-id="746fa-113">Du skal finde og føje disse websteder til listen over virksomhedswebsteder, så du kun kan bruge Internet Explorer-tilstand til disse websteder.</span><span class="sxs-lookup"><span data-stu-id="746fa-113">You'll want to find and add these sites to the Enterprise Site List so that you can use Internet Explorer mode only for those sites.</span></span>

> [!NOTE]
> <span data-ttu-id="746fa-114">[Enterprise Site Discovery finder](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) websteder, der muligvis skal bruge Internet Explorer-tilstand.</span><span class="sxs-lookup"><span data-stu-id="746fa-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) discovers sites that might need Internet Explorer mode.</span></span> <span data-ttu-id="746fa-115">Det kan indsamle data på computere, der kører Windows Internet Explorer 8 via Internet Explorer 11 på Windows 10, Windows 8.1 eller Windows 7.</span><span class="sxs-lookup"><span data-stu-id="746fa-115">It can collect data on computers running Windows Internet Explorer 8 through Internet Explorer 11 on Windows 10, Windows 8.1, or Windows 7.</span></span>

<span data-ttu-id="746fa-116">**Analysér dataene**</span><span class="sxs-lookup"><span data-stu-id="746fa-116">**Analyze the data**</span></span>

<span data-ttu-id="746fa-117">Når du har indsamlet webstedsdata, anbefaler vi følgende proces i fire trin for at analysere dataene:</span><span class="sxs-lookup"><span data-stu-id="746fa-117">After you've collected site data, we recommend the following four-step process to analyze the data:</span></span>
1. <span data-ttu-id="746fa-118">Sortér dataene efter domæne og derefter efter URL-adresse.</span><span class="sxs-lookup"><span data-stu-id="746fa-118">Sort the data by domain, and then by URL.</span></span>
2. <span data-ttu-id="746fa-119">Definer grænserne for en app, der skal konfigureres i Internet Explorer-tilstand.</span><span class="sxs-lookup"><span data-stu-id="746fa-119">Define the boundaries of an app to configure for Internet Explorer mode.</span></span> <span data-ttu-id="746fa-120">Du vil medtage alle de websteder og webkontrolelementer, der definerer appen, men du vil ikke inkludere ekstra websteder og kontrolelementer.</span><span class="sxs-lookup"><span data-stu-id="746fa-120">You want to include all the sites and web controls that define the app, but you don't want to include extra sites and controls.</span></span> <span data-ttu-id="746fa-121">Nogle websteder kan være så enkle, som *https://contoso.com/app1* mens andre muligvis kræver, at du definerer flere websteder og sider.</span><span class="sxs-lookup"><span data-stu-id="746fa-121">Some sites might be as simple as *https://contoso.com/app1* while others might require you to define multiple sites and pages.</span></span>
3. <span data-ttu-id="746fa-122">Test appen for at bekræfte, at den ikke fungerer oprindeligt.</span><span class="sxs-lookup"><span data-stu-id="746fa-122">Test the app to verify that it doesn't work natively.</span></span> <span data-ttu-id="746fa-123">Mange websteder tilbyder moderne indhold, når de registrerer en moderne browser og tilbyder kun ældre indhold, når de registrerer Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="746fa-123">Many sites will offer modern content when they detect a modern browser and only offer legacy content when they detect Internet Explorer.</span></span>
4. <span data-ttu-id="746fa-124">Føj appen til din enterprise-webstedsliste, hvis det mislykkes at teste.</span><span class="sxs-lookup"><span data-stu-id="746fa-124">Add the app to your Enterprise Site List if it fails testing.</span></span>

> [!NOTE]
> <span data-ttu-id="746fa-125">Som bedste fremgangsmåde skal du gruppere alle de websteder, der udgør en app.</span><span class="sxs-lookup"><span data-stu-id="746fa-125">As a best practice, group all of the sites that comprise an app.</span></span> <span data-ttu-id="746fa-126">På denne måde er det nemmere, når du opgraderer en app, at fjerne hele webstedet fra Internet Explorer-tilstand og begynde at bruge en moderne browser til den pågældende app.</span><span class="sxs-lookup"><span data-stu-id="746fa-126">This way, when you upgrade an app, it's easier to remove the entire site from Internet Explorer mode and start using a modern browser for that app.</span></span>

<span data-ttu-id="746fa-127">Når du er færdig med webstedsregistreringen, og du har analyseret dataene, er du klar til at begynde at kigge på din kanalstrategi.</span><span class="sxs-lookup"><span data-stu-id="746fa-127">Once you're done with site discovery and you've analyzed the data, you're ready to start looking at your channel strategy.</span></span>

