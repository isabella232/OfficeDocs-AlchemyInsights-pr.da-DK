---
title: Arbejds- og arbejdsmail sendes ikke
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 391d3a2dcc2676a405065115f375c802d2492119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766127"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="89078-102">Der sendes ikke en mail til en SharePoint-liste eller et SharePoint-bibliotek</span><span class="sxs-lookup"><span data-stu-id="89078-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="89078-103">Mails fra arbejdsprocesser sendes ikke til alle brugere eller kun bestemte brugere, eller du får vist fejlen **E-mailen kan ikke sendes. Sørg for, at e-mailen har en gyldig modtager**.</span><span class="sxs-lookup"><span data-stu-id="89078-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="89078-104">Kontroller, om brugeren findes i gruppen Alle **personers** tilladelser (liste over brugeroplysninger) for den pågældende gruppe af websteder.</span><span class="sxs-lookup"><span data-stu-id="89078-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="89078-105">Eksempel på direkte<tenant>URL-adresse: https:// .sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MedlemskabGroupId=0</span><span class="sxs-lookup"><span data-stu-id="89078-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="89078-106">Hvis brugeren ikke findes, skal du kontrollere, at brugeren er logget på siden.</span><span class="sxs-lookup"><span data-stu-id="89078-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="89078-107">Hvis det er en ekstern bruger, skal du sørge for, at invitationen er blevet accepteret.</span><span class="sxs-lookup"><span data-stu-id="89078-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="89078-108">Hvis brugeren findes i tilladelsesgruppen, skal du kontrollere, at mailadressen er korrekt.</span><span class="sxs-lookup"><span data-stu-id="89078-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="89078-109">Hvis brugernes mailadresse ikke er angivet her, skal du oprette en eksempelbesked for den pågældende bruger, som gennemtvinger synkroniseringen af den pågældende brugerkonto fra Brugerprofiler af SharePoint til denne gruppe af websteder.</span><span class="sxs-lookup"><span data-stu-id="89078-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="89078-110">Mails fra arbejdsprocesser sendes til administratorer af gruppen af websteder, men ikke til andre brugere, og fejlen **HTTP Forbidden til <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span><span class="sxs-lookup"><span data-stu-id="89078-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="89078-111">Se [Adgang nægtet, når du sender en mail til en SharePoint-gruppe](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="89078-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="89078-112">Kontroller også, at funktionen Låsning af **brugertilladelse** med begrænset adgang ikke er aktiv.</span><span class="sxs-lookup"><span data-stu-id="89078-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="89078-113">Relaterede emner</span><span class="sxs-lookup"><span data-stu-id="89078-113">Related topics</span></span>
<span data-ttu-id="89078-114">Vil du prøve Microsoft Flow i SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="89078-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="89078-115">Opret flow</span><span class="sxs-lookup"><span data-stu-id="89078-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="89078-116">SharePoint og Flow</span><span class="sxs-lookup"><span data-stu-id="89078-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


