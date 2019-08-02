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
# <a name="workflow-email-is-not-being-sent"></a>Arbejdsprocessen e-mail sendes ikke

1. E-mail fra arbejdsprocesser sendes ikke til alle brugere eller kun bestemte brugere, eller du kan se fejlen **e-mail-meddelelsen ikke kan sendes. Kontroller, at e-mail har et gyldigt**.

Marker, hvis brugeren findes i gruppen **Alle** tilladelser (listen med brugeroplysninger) for denne gruppe af websteder.  Eksempel på direkte URL-adresse: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0

- Hvis brugeren ikke findes, Kontroller, at brugeren er logget på siden. 
- Hvis det er en ekstern bruger, Sørg for, at deres invitation er accepteret.
- Hvis brugeren findes i gruppen tilladelser, skal du kontrollere e-mail-adresse er korrekt.
- Hvis brugere e-mail-adressen ikke er angivet her, skal du oprette et eksempel på en skrivebordsbesked for den pågældende bruger, som gennemtvinger synkronisering af denne brugerkonto fra SharePoint bruger profiler til denne gruppe af websteder.
 
2. E-mail fra arbejdsprocesser sendes til SharePoint Designer, men ikke til andre brugere og se fejlen **http-forbudt at <spam> <spam> ** <spam> <spam>.
 

Se [Adgang nægtet, når sendt e-mail til grupper](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).

Du skal også kontrollere, at funktionen **begrænset adgang tilladelse lockdown brugertilstand** websted websteder ikke er aktiv.

## <a name="related-topics"></a>Relaterede emner
- [Oprette produktionsflow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint og Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


