---
title: Grænsen for daglige mails er overskredet. Arbejdsprocessen er suspenderet.
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
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731557"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Grænsen for daglige mails er overskredet. Arbejdsprocessen er suspenderet.

Denne fejl kan være modtaget i følgende scenarier:

- Du har en arbejdsproces i SharePoint Online, der bruger SharePoint 2010-eller SharePoint 2013-typen arbejdsproces platform.
- Arbejdsprocessen er konfigureret til at sende en brugerdefineret mail til mere end 200 brugere ad gangen, mere end 10.000 modtagere pr. dag eller mere end 30 meddelelser pr. minut.
- Når du kører arbejdsprocessen, bliver mail meddelelsen ikke sendt, og du bemærker følgende funktionsmåde:
    - For en arbejdsproces, der bruger typen SharePoint 2013-platform, skal du gå til siden **status for arbejdsproces** . På siden status for arbejdsproces er den **interne status** angivet til **Startet**, og oplysnings boblen vises ikke, så du kan **sende til en modtager**.

Du kan løse dette problem ved at konfigurere arbejdsprocessen til at sende mails uden at overskride [begrænsningerne for Exchange Online-afsenderen](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). For eksempel skal du bruge en pause i arbejdsprocessen, sende mailen til en Microsoft 365-gruppe, en distributionsgruppe eller en e-mail-aktiveret sikkerhedsgruppe eller sende meddelelsen til færre end 200 modtagere ad gangen.


Du kan finde flere oplysninger i følgende [artikel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Relaterede emner
- [Opret flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint og flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 