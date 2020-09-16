---
title: Arbejdsproces mail sendes ikke
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748983"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="1f7a1-102">Arbejdsproces mail sendes ikke for en SharePoint-liste eller et bibliotek</span><span class="sxs-lookup"><span data-stu-id="1f7a1-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="1f7a1-103">Mail fra arbejdsprocesser sendes ikke til alle brugere eller kun bestemte brugere, eller du får vist en fejl **meddelelse om, at mailen ikke kan sendes. Sørg for, at mailen har en gyldig modtager**.</span><span class="sxs-lookup"><span data-stu-id="1f7a1-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="1f7a1-104">Kontrollér, om brugeren findes i gruppen **alle** tilladelser til personer (listen med brugeroplysninger) for den pågældende gruppe af websteder.</span><span class="sxs-lookup"><span data-stu-id="1f7a1-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="1f7a1-105">Eksempel på Direct URL-adresse: https:// <tenant> . SharePoint.com/sites/ <sitename> /_layouts/15/People.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="1f7a1-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="1f7a1-106">Hvis brugeren ikke findes, skal du kontrollere, at brugeren er logget på siden.</span><span class="sxs-lookup"><span data-stu-id="1f7a1-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="1f7a1-107">Hvis det er en ekstern bruger, skal du sørge for, at vedkommendes invitation er blevet accepteret.</span><span class="sxs-lookup"><span data-stu-id="1f7a1-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="1f7a1-108">Hvis brugeren findes i gruppen tilladelser, skal du sørge for, at e-mail-adressen er korrekt.</span><span class="sxs-lookup"><span data-stu-id="1f7a1-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="1f7a1-109">Hvis brugerens mailadresse ikke er angivet her, skal du oprette en eksempel besked for den pågældende bruger, der gennemtvinger synkronisering af den pågældende brugerkonto fra brugerprofiler i SharePoint til denne gruppe af websteder.</span><span class="sxs-lookup"><span data-stu-id="1f7a1-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="1f7a1-110">Mail fra arbejdsprocesser sendes til administratorerne af gruppen af websteder, men ikke til andre brugere, og de kan se fejlen **http forbudt til <span>https:</span>//URL/_vti_bin/Client.xvc.Sp.Utilities.Utility.SendEmail**.</span><span class="sxs-lookup"><span data-stu-id="1f7a1-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="1f7a1-111">Se [adgang nægtet, når du sender en mail til en SharePoint-gruppe](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="1f7a1-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="1f7a1-112">Du skal også bekræfte, at funktionen til gruppe af websteder med **begrænset adgang til brugertilladelser** ikke er aktiv.</span><span class="sxs-lookup"><span data-stu-id="1f7a1-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="1f7a1-113">Relaterede emner</span><span class="sxs-lookup"><span data-stu-id="1f7a1-113">Related topics</span></span>
<span data-ttu-id="1f7a1-114">Vil du prøve Microsoft flow i SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="1f7a1-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="1f7a1-115">Opret flow</span><span class="sxs-lookup"><span data-stu-id="1f7a1-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="1f7a1-116">SharePoint og flow</span><span class="sxs-lookup"><span data-stu-id="1f7a1-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


