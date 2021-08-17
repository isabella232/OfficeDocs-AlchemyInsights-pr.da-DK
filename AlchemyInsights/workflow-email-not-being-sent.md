---
title: Arbejdsprocesmail sendes ikke
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
ms.openlocfilehash: 2caf8e0878da0049667d9a19f4488eaec4b9327fbf36be7d29dbf4b7a9c89158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072514"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Arbejdsprocesmail sendes ikke til en liste eller SharePoint et bibliotek

1. Mail fra arbejdsprocesser sendes ikke til alle brugere eller kun bestemte brugere, eller du får vist fejlen Mailen kan ikke sendes. Sørg for, at mailen har en **gyldig modtager.**

    Kontrollér, om brugeren findes i **tilladelsesgruppen Alle** personer (listen brugeroplysninger) for den pågældende gruppe af websteder.  Eksempel på en direkte URL-adresse: <tenant> https:// .sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx? MembershipGroupId=0

    - Hvis brugeren ikke findes, skal du kontrollere, at brugeren er logget på siden. 
    - Hvis det er en ekstern bruger, skal du kontrollere, at invitationen er blevet accepteret.
    - Hvis brugeren findes i tilladelsesgruppen, skal du kontrollere, at mailadressen er korrekt.
    - Hvis brugerens mailadresse ikke er angivet her, skal du oprette en eksempelbesked for den pågældende bruger, som tvinger synkroniseringen af den pågældende brugerkonto fra Brugerprofiler SharePoint denne gruppe af websteder.
 
2. Mail fra arbejdsprocesser sendes til administratorer af grupper af websteder, men ikke til andre brugere, og fejlen **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Se [Adgang nægtet, når du sender en mail til SharePoint gruppe.](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)

    Bekræft også, at funktionen **Låst tilstand for** brugere med tilladelsen Begrænset adgang ikke er aktiv.


## <a name="related-topics"></a>Relaterede emner
Vil du prøve Microsoft Flow i SharePoint Online?
- [Opret Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint og Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


