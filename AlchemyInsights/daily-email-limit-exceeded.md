---
title: Den daglige e-mail grænse er overskredet. Arbejdsprocessen er afbrudt.
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
ms.openlocfilehash: 3cad5d8305da0a5db9a85888793350a062e6aed6
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053111"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Den daglige e-mail grænse er overskredet. Arbejdsprocessen er afbrudt.

Denne fejl kan blive modtaget i følgende scenarier:

- Du har en arbejdsproces i SharePoint Online, der bruger SharePoint 2010-eller SharePoint 2013-arbejdsgangs platforms typen.
- Arbejdsprocessen er konfigureret til at sende en brugerdefineret e-mail-meddelelse til mere end 200 brugere ad gangen, mere end 10.000 modtagere pr. dag eller mere end 30 meddelelser pr. minut.
- Når du kører arbejdsprocessen, sendes e-mailen ikke, og du bemærker følgende funktionsmåde:
    - For en arbejdsproces, der bruger SharePoint 2013-platforms typen, skal du gå til siden **status for arbejdsproces** . På siden status for arbejdsproces er den **interne status** angivet til **Startet**, og informations ballonen viser, at den **ikke kan sende til en modtager**.

Du skal løse dette problem ved at konfigurere arbejdsprocessen til at sende mails uden at overskride [grænserne for afsenderens Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)-meddelelser. Bruge en pause i arbejdsprocessen, sende mailen til en Office 365-gruppe, en distributionsgruppe eller en sikkerhedsgruppe med post aktiveret eller sende meddelelsen til færre end 200 modtagere ad gangen.


Yderligere oplysninger finder du i følgende [artikel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Relaterede emner
- [Opret flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint og flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 