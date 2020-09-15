---
title: Skrivebeskyttet for vedligeholdelses meddelelse, når du forsøger at bruge SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670826"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="f07a5-102">Skrivebeskyttet for vedligeholdelses meddelelse, når du forsøger at bruge SharePoint eller OneDrive</span><span class="sxs-lookup"><span data-stu-id="f07a5-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="f07a5-103">Brugere kan modtage en **skrivebeskyttet til vedligeholdelses** meddelelse, når de forsøger at bruge SharePoint eller OneDrive til en af følgende scenarier.</span><span class="sxs-lookup"><span data-stu-id="f07a5-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="f07a5-104">En planlagt eller aktiv vedligeholdelses aktivitet.</span><span class="sxs-lookup"><span data-stu-id="f07a5-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="f07a5-105">Du kan søge efter dem ved at gå til [meddelelses Center](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="f07a5-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="f07a5-106">En høj prioritet, aktiv tjeneste hændelse, der kan forekomme.</span><span class="sxs-lookup"><span data-stu-id="f07a5-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="f07a5-107">Kontrollér, om der er rådgivere/Incidents ved at navigere til [tjenestetilstand](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="f07a5-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="f07a5-108">Et mindre automatisk reparerende genoprettelses scenarie, der kan ske på grund af eventuelle uventede begivenheder på de servere, der muligvis er på under 30 min.</span><span class="sxs-lookup"><span data-stu-id="f07a5-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="f07a5-109">Der er ingen meddelelses Center-eller tjeneste Tilstandsposter for disse mindre regress, men du bør snart være tilbage til normal.</span><span class="sxs-lookup"><span data-stu-id="f07a5-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="f07a5-110">I ganske få tilfælde observerede vi, at et af de tre scenarier, der er nævnt ovenfor, har været årsag til, at tjenesten er blevet gendannet, men browserens browsercache er ikke blevet ryddet op.</span><span class="sxs-lookup"><span data-stu-id="f07a5-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="f07a5-111">Prøv at rydde browsercachen, før du navigerer til webstedet.</span><span class="sxs-lookup"><span data-stu-id="f07a5-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="f07a5-112">Vælg **Indstillinger**i din Microsoft Edge-browser, og vælg derefter **beskyttelse af personlige oplysninger og sikkerhed**.</span><span class="sxs-lookup"><span data-stu-id="f07a5-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="f07a5-113">Under **Ryd browsing**skal du vælge **Vælg det, der skal ryddes**.</span><span class="sxs-lookup"><span data-stu-id="f07a5-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="f07a5-114">Vælg **cookies og gemte webstedsdata**, og vælg **Ryd**.</span><span class="sxs-lookup"><span data-stu-id="f07a5-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="f07a5-115">Disse trin kan være forskellige, når du bruger andre browsere som Mozilla Firefox eller Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="f07a5-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="f07a5-116">En anden mulighed er at åbne dit SharePoint-websted eller OneDrive i et nyt InPrivate-vindue.</span><span class="sxs-lookup"><span data-stu-id="f07a5-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>