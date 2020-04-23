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
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Der sendes ikke en mail til en SharePoint-liste eller et SharePoint-bibliotek

1. Mails fra arbejdsprocesser sendes ikke til alle brugere eller kun bestemte brugere, eller du får vist fejlen **E-mailen kan ikke sendes. Sørg for, at e-mailen har en gyldig modtager**.

    Kontroller, om brugeren findes i gruppen Alle **personers** tilladelser (liste over brugeroplysninger) for den pågældende gruppe af websteder.  Eksempel på direkte<tenant>URL-adresse: https:// .sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MedlemskabGroupId=0

    - Hvis brugeren ikke findes, skal du kontrollere, at brugeren er logget på siden. 
    - Hvis det er en ekstern bruger, skal du sørge for, at invitationen er blevet accepteret.
    - Hvis brugeren findes i tilladelsesgruppen, skal du kontrollere, at mailadressen er korrekt.
    - Hvis brugernes mailadresse ikke er angivet her, skal du oprette en eksempelbesked for den pågældende bruger, som gennemtvinger synkroniseringen af den pågældende brugerkonto fra Brugerprofiler af SharePoint til denne gruppe af websteder.
 
2. Mails fra arbejdsprocesser sendes til administratorer af gruppen af websteder, men ikke til andre brugere, og fejlen **HTTP Forbidden til <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Se [Adgang nægtet, når du sender en mail til en SharePoint-gruppe](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Kontroller også, at funktionen Låsning af **brugertilladelse** med begrænset adgang ikke er aktiv.


## <a name="related-topics"></a>Relaterede emner
Vil du prøve Microsoft Flow i SharePoint Online?
- [Opret flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint og Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


