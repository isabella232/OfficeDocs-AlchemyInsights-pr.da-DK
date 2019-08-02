---
title: Arbejdsprocessen e-mail sendes ikke
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 783bf0a5721aa5db7088432c71e06cac6dc90513
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059598"
---
# <a name="workflow-email-is-not-being-sent"></a><span data-ttu-id="1a6e3-102">Arbejdsprocessen e-mail sendes ikke</span><span class="sxs-lookup"><span data-stu-id="1a6e3-102">Workflow email is not being sent</span></span>

1. <span data-ttu-id="1a6e3-103">E-mail fra arbejdsprocesser sendes ikke til alle brugere eller kun bestemte brugere, eller du kan se fejlen **e-mail-meddelelsen ikke kan sendes. Kontroller, at e-mail har et gyldigt**.</span><span class="sxs-lookup"><span data-stu-id="1a6e3-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

<span data-ttu-id="1a6e3-104">Marker, hvis brugeren findes i gruppen **Alle** tilladelser (listen med brugeroplysninger) for denne gruppe af websteder.</span><span class="sxs-lookup"><span data-stu-id="1a6e3-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="1a6e3-105">Eksempel på direkte URL-adresse: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="1a6e3-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

- <span data-ttu-id="1a6e3-106">Hvis brugeren ikke findes, Kontroller, at brugeren er logget på siden.</span><span class="sxs-lookup"><span data-stu-id="1a6e3-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
- <span data-ttu-id="1a6e3-107">Hvis det er en ekstern bruger, Sørg for, at deres invitation er accepteret.</span><span class="sxs-lookup"><span data-stu-id="1a6e3-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
- <span data-ttu-id="1a6e3-108">Hvis brugeren findes i gruppen tilladelser, skal du kontrollere e-mail-adresse er korrekt.</span><span class="sxs-lookup"><span data-stu-id="1a6e3-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
- <span data-ttu-id="1a6e3-109">Hvis brugere e-mail-adressen ikke er angivet her, skal du oprette et eksempel på en skrivebordsbesked for den pågældende bruger, som gennemtvinger synkronisering af denne brugerkonto fra SharePoint bruger profiler til denne gruppe af websteder.</span><span class="sxs-lookup"><span data-stu-id="1a6e3-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="1a6e3-110">E-mail fra arbejdsprocesser sendes til SharePoint Designer, men ikke til andre brugere og se fejlen \*\*http-forbudt at <spam> <spam> \*\* <spam> <spam>.</span><span class="sxs-lookup"><span data-stu-id="1a6e3-110">Email from Workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <spam><spam>https://URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**<spam><spam>.</span></span>
 

<span data-ttu-id="1a6e3-111">Se [Adgang nægtet, når sendt e-mail til grupper](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="1a6e3-111">See [Access Denied when sent email to groups](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span></span>

<span data-ttu-id="1a6e3-112">Du skal også kontrollere, at funktionen **begrænset adgang tilladelse lockdown brugertilstand** websted websteder ikke er aktiv.</span><span class="sxs-lookup"><span data-stu-id="1a6e3-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>

## <a name="related-topics"></a><span data-ttu-id="1a6e3-113">Relaterede emner</span><span class="sxs-lookup"><span data-stu-id="1a6e3-113">Related topics</span></span>
- [<span data-ttu-id="1a6e3-114">Oprette produktionsflow</span><span class="sxs-lookup"><span data-stu-id="1a6e3-114">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="1a6e3-115">SharePoint og Flow</span><span class="sxs-lookup"><span data-stu-id="1a6e3-115">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


