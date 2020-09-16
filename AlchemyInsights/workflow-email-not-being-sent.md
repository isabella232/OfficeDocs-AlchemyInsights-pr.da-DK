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
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Arbejdsproces mail sendes ikke for en SharePoint-liste eller et bibliotek

1. Mail fra arbejdsprocesser sendes ikke til alle brugere eller kun bestemte brugere, eller du får vist en fejl **meddelelse om, at mailen ikke kan sendes. Sørg for, at mailen har en gyldig modtager**.

    Kontrollér, om brugeren findes i gruppen **alle** tilladelser til personer (listen med brugeroplysninger) for den pågældende gruppe af websteder.  Eksempel på Direct URL-adresse: https:// <tenant> . SharePoint.com/sites/ <sitename> /_layouts/15/People.aspx? MembershipGroupId = 0

    - Hvis brugeren ikke findes, skal du kontrollere, at brugeren er logget på siden. 
    - Hvis det er en ekstern bruger, skal du sørge for, at vedkommendes invitation er blevet accepteret.
    - Hvis brugeren findes i gruppen tilladelser, skal du sørge for, at e-mail-adressen er korrekt.
    - Hvis brugerens mailadresse ikke er angivet her, skal du oprette en eksempel besked for den pågældende bruger, der gennemtvinger synkronisering af den pågældende brugerkonto fra brugerprofiler i SharePoint til denne gruppe af websteder.
 
2. Mail fra arbejdsprocesser sendes til administratorerne af gruppen af websteder, men ikke til andre brugere, og de kan se fejlen **http forbudt til <span>https:</span>//URL/_vti_bin/Client.xvc.Sp.Utilities.Utility.SendEmail**.
 

    Se [adgang nægtet, når du sender en mail til en SharePoint-gruppe](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Du skal også bekræfte, at funktionen til gruppe af websteder med **begrænset adgang til brugertilladelser** ikke er aktiv.


## <a name="related-topics"></a>Relaterede emner
Vil du prøve Microsoft flow i SharePoint Online?
- [Opret flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint og flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


