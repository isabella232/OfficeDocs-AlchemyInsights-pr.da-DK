---
title: Daglig mailgrænse overskredet. Arbejdsprocessen er afbrudt.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 60ddbe68298e998a4e0b271a15209efc135c80638702c98dbcb3e0b2f1554860
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914645"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Daglig mailgrænse overskredet. Arbejdsprocessen er afbrudt.

Denne fejl kan opstå i følgende scenarier:

- Du har en arbejdsproces i SharePoint Online, der bruger SharePoint 2010 eller SharePoint 2013-arbejdsprocesplatformtypen.
- Arbejdsprocessen er konfigureret til at sende en brugerdefineret mail til mere end 200 brugere ad gangen, mere end 10.000 modtagere pr. dag eller mere end 30 meddelelser i minuttet.
- Når du kører arbejdsprocessen, sendes mailen ikke, og du bemærker følgende funktionsmåde:
    - Hvis du vil have en arbejdsproces, der SharePoint 2013-platformtypen, skal du gå til **siden Status for** arbejdsproces. På siden Status for arbejdsproces er Den **interne status** angivet til Startet **,** og informationsboblen viser Kan ikke sende til **en modtager**.

Du kan løse dette problem ved at konfigurere arbejdsprocessen til at sende mails uden at Exchange Online [af afsenderbegrænsningerne.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits) Brug f.eks. en pause i arbejdsprocessen, send mailen til en Microsoft 365-gruppe, en distributionsgruppe eller mailaktiveret sikkerhedsgruppe, eller send meddelelsen til færre end 200 modtagere ad gangen.


Du kan finde flere oplysninger i følgende [artikel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Relaterede emner
- [Opret Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint og Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 