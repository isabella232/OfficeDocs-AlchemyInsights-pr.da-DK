---
title: E-mail i arbejdsgangen sendes ikke
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 76b64323c9d34d49e9c6bd77c2cc7eff6d7c5402
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049367"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Arbejdsgang-e-mail sendes ikke til en SharePoint-liste eller et bibliotek

1. Mails fra arbejdsprocesser sendes ikke til alle brugere eller kun til bestemte brugere, eller der vises en fejl **meddelelse om, at e-mailen ikke kan sendes. Kontroller, at e-mailen har en gyldig modtager**.

    Kontroller, om brugeren findes i gruppen **alle personer** -tilladelser (liste over brugeroplysninger) for den pågældende gruppe af websteder.  Eksempel på direkte webadresse:<tenant>https://.<sitename>SharePoint.com/sites//_layouts/15/People.aspx? MembershipGroupId = 0

    - Hvis brugeren ikke findes, skal du kontrollere, at brugeren er logget på siden. 
    - Hvis det er en ekstern bruger, skal du sørge for, at invitationen er accepteret.
    - Hvis brugeren findes i gruppen tilladelser, skal du kontrollere, at e-mail-adressen er korrekt.
    - Hvis brugerens e-mailadresse ikke er angivet her, skal du oprette en eksempel besked for den bruger, der tvinger synkroniseringen af den pågældende brugerkonto fra brugerprofiler i SharePoint til denne gruppe af websteder.
 
2. Mails fra arbejdsprocesser sendes til administratorer af gruppen af websteder, men ikke til andre brugere, og der vises en fejl **http-forbudt <span>https:</span>/url/_vti_bin/Client.xvc.Sp.Utilities.Utility.SendEmail**.
 

    Se [adgang nægtet, når du sender en mail til en SharePoint-gruppe](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Du skal også kontrollere, at funktionen for gruppe af **brugertilladelser med begrænset adgang** ikke er aktiv.


## <a name="related-topics"></a>Relaterede emner
Vil du prøve Microsoft flow i SharePoint Online?
- [Opret flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint og flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


