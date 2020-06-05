---
title: Den daglige e-mail-grænse er overskredet. Arbejdsprocessen er afbrudt.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 701c4aef6bfc0c4a2c4570f6dd16dbe4f99efc44
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580327"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Den daglige e-mail-grænse er overskredet. Arbejdsprocessen er afbrudt.

Denne fejl kan modtages i følgende scenarier:

- Du har en arbejdsproces i SharePoint Online, der bruger statustypen SharePoint 2010- eller SharePoint 2013-arbejdsprocesplatform.
- Arbejdsprocessen er konfigureret til at sende en brugerdefineret mail til mere end 200 brugere ad gangen, mere end 10.000 modtagere om dagen eller mere end 30 meddelelser i minuttet.
- Når du kører arbejdsprocessen, sendes mailen ikke, og du bemærker følgende funktionsmåde:
    - For en arbejdsproces, der bruger sharepoint 2013-platformtypen, skal du gå til **siden Status for arbejdsproces.** På siden Status for arbejdsproces er den **interne status** angivet til **Startet**, og informationsboblen **viser, at den ikke kan sendes til en modtager**.

Du kan løse dette problem ved at konfigurere arbejdsprocessen til at sende mails uden at overskride [grænserne for Exchange Online-afsenderen](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). bruge en pause i arbejdsprocessen, sende mailen til en Microsoft 365-gruppe, en distributionsgruppe eller en mailaktiveret sikkerhedsgruppe eller sende meddelelsen til færre end 200 modtagere ad gangen.


Yderligere oplysninger finder du i følgende [artikel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Relaterede emner
- [Opret flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint og Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 