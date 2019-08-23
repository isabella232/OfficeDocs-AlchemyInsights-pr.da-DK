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
ms.openlocfilehash: 261fe1b1bc815dd4ad568051cfefad1e214b957e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530861"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Arbejdsprocessen e-mail sendes ikke til en SharePoint-liste eller et bibliotek

1. E-mail fra arbejdsprocesser sendes ikke til alle brugere eller kun bestemte brugere, eller du kan se fejlen **e-mail-meddelelsen ikke kan sendes. Kontroller, at e-mail har et gyldigt**.

    Marker, hvis brugeren findes i gruppen **Alle** tilladelser (listen med brugeroplysninger) for denne gruppe af websteder.  Eksempel på direkte URL-adresse: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0

    - Hvis brugeren ikke findes, Kontroller, at brugeren er logget på siden. 
    - Hvis det er en ekstern bruger, Sørg for, at deres invitation er accepteret.
    - Hvis brugeren findes i gruppen tilladelser, skal du kontrollere e-mail-adresse er korrekt.
    - Hvis brugere e-mail-adressen ikke er angivet her, skal du oprette et eksempel på en skrivebordsbesked for den pågældende bruger, som gennemtvinger synkronisering af denne brugerkonto fra SharePoint bruger profiler til denne gruppe af websteder.
 
2. E-mail fra arbejdsprocesser sendes til SharePoint Designer, men ikke til andre brugere og se fejlen **http-forbudt at <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Se [Adgang nægtet, når du sender en e-mail til en SharePoint-gruppe](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Du skal også kontrollere, at funktionen **begrænset adgang tilladelse lockdown brugertilstand** websted websteder ikke er aktiv.


## <a name="related-topics"></a>Relaterede emner
Vil du prøve Microsoft Flow i SharePoint Online?
- [Oprette produktionsflow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint og Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


