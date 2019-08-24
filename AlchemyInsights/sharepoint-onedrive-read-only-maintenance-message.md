---
title: Skrivebeskyttet for vedligeholdelse, når du forsøger at bruge SharePoint- eller OneDrive
ms.author: efrene
author: efrene
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
ms.openlocfilehash: 5b1e56253d6deeb0f9ba2f753eff5c00ff9c51a2
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620717"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="7dcc6-102">Skrivebeskyttet for vedligeholdelse, når du forsøger at bruge SharePoint- eller OneDrive</span><span class="sxs-lookup"><span data-stu-id="7dcc6-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="7dcc6-103">Brugere kan modtager meddelelsen **Skrivebeskyttet for vedligeholdelse** , når du forsøger at bruge SharePoint- eller OneDrive til en af følgende situationer.</span><span class="sxs-lookup"><span data-stu-id="7dcc6-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="7dcc6-104">En planlagt eller aktiv vedligeholdelse aktivitet.</span><span class="sxs-lookup"><span data-stu-id="7dcc6-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="7dcc6-105">Søge efter dem ved at gå til [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="7dcc6-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="7dcc6-106">En høj prioritet, aktiv tjeneste hændelse, der kan forekomme.</span><span class="sxs-lookup"><span data-stu-id="7dcc6-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="7dcc6-107">Kontrollere, om eventuelle råd om hændelser ved at navigere til [Service sundhed](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="7dcc6-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="7dcc6-108">En mindre automatisk reparationspenselværktøjet nedbrud, der kunne ske noget på grund af uventede hændelser på de servere, som måske sidste for mindre end 30 min. eller så.</span><span class="sxs-lookup"><span data-stu-id="7dcc6-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="7dcc6-109">Der er ingen meddelelse Center eller Service sundhed bogføres for disse mindre tilbagebetalinger, men du skal være tilbage til normal snart.</span><span class="sxs-lookup"><span data-stu-id="7dcc6-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="7dcc6-110">I meget få tilfælde konstaterede vi, at et af de tre scenarier, der er anført ovenfor, er årsagen, og service er blevet gendannet, men browsercachen brugerne endnu ikke ryddet.</span><span class="sxs-lookup"><span data-stu-id="7dcc6-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="7dcc6-111">Du bør forsøge at rydde browsercachen før navigere til webstedet.</span><span class="sxs-lookup"><span data-stu-id="7dcc6-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="7dcc6-112">Vælg **Indstillinger**i browseren Microsoft Edge, og vælg derefter **personlige oplysninger og sikkerhed**.</span><span class="sxs-lookup"><span data-stu-id="7dcc6-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="7dcc6-113">Vælg **vælge Ryd**under **Ryd søgning**.</span><span class="sxs-lookup"><span data-stu-id="7dcc6-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="7dcc6-114">Vælg **Cookies og gemt webstedet data**, og vælg **Slet**.</span><span class="sxs-lookup"><span data-stu-id="7dcc6-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="7dcc6-115">Disse trin kan variere, når du bruger andre browsere som Mozilla Firefox eller Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="7dcc6-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="7dcc6-116">En anden mulighed ville være at åbne SharePoint-webstedet eller OneDrive i et nyt InPrivate-vindue.</span><span class="sxs-lookup"><span data-stu-id="7dcc6-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>