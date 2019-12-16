---
title: Skrivebeskyttet for vedligeholdelses meddelelse, når du forsøger at bruge SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051275"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="39669-102">Skrivebeskyttet for vedligeholdelses meddelelse, når du forsøger at bruge SharePoint eller OneDrive</span><span class="sxs-lookup"><span data-stu-id="39669-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="39669-103">Brugere kan modtage en **skrivebeskyttet meddelelse om vedligeholdelse** , når de forsøger at bruge SharePoint eller OneDrive til et af følgende scenarier.</span><span class="sxs-lookup"><span data-stu-id="39669-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="39669-104">En planlagt eller aktiv vedligeholdelsesaktivitet.</span><span class="sxs-lookup"><span data-stu-id="39669-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="39669-105">Tjek for dem ved at navigere til [meddelelsescenteret](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="39669-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="39669-106">En aktiv tjeneste hændelse med høj prioritet, der kan forekomme.</span><span class="sxs-lookup"><span data-stu-id="39669-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="39669-107">Søg efter meddelelser/hændelser ved at navigere til [tjenestens tilstand](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="39669-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="39669-108">En mindre Auto-healing opsving scenario, der kunne ske på grund af uventede begivenheder på serverne, som kan vare mindre end 30 min eller deromkring.</span><span class="sxs-lookup"><span data-stu-id="39669-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="39669-109">Der er ingen Message Center eller service Health posts for disse mindre inddrivelser, men du skal være tilbage til normal meget snart.</span><span class="sxs-lookup"><span data-stu-id="39669-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="39669-110">Ved meget få lejligheder bemærkede vi, at en af de tre scenarier, der er anført ovenfor har været årsag, og tjenesten er blevet genoprettet, men brugerne browser cache er ikke blevet ryddet op.</span><span class="sxs-lookup"><span data-stu-id="39669-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="39669-111">Forsøg at rydde browserens cache, før du navigerer til webstedet.</span><span class="sxs-lookup"><span data-stu-id="39669-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="39669-112">I din Microsoft Edge-browser skal du vælge **Indstillinger**og derefter vælge **beskyttelse af personlige oplysninger og sikkerhed**.</span><span class="sxs-lookup"><span data-stu-id="39669-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="39669-113">Under **Ryd browsing**skal du vælge **Vælg, hvad du vil rydde**.</span><span class="sxs-lookup"><span data-stu-id="39669-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="39669-114">Vælg **cookies og gemte webstedsdata**, og vælg **Ryd**.</span><span class="sxs-lookup"><span data-stu-id="39669-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="39669-115">Disse trin kan afvige, når du bruger andre browsere som Mozilla Firefox eller Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="39669-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="39669-116">En anden mulighed ville være at åbne dit SharePoint-websted eller OneDrive i et nyt InPrivate-vindue.</span><span class="sxs-lookup"><span data-stu-id="39669-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>