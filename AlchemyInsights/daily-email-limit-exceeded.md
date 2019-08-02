---
title: Daglige e-mail-grænse er overskredet. Arbejdsprocessen er afbrudt.
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
- "1227"
ms.openlocfilehash: 802aba696da61be5f0a6c12072842cbc3cd96499
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059633"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Daglige e-mail, der er overskredet. Arbejdsprocessen er afbrudt.

Denne fejl kan modtages i følgende situationer:

- Du har en arbejdsproces i SharePoint Online, der bruger SharePoint 2010 eller SharePoint 2013 platform arbejdsgangstype.
- Arbejdsgangen er konfigureret til at sende en brugerdefineret e-mail-meddelelse til mere end 200 brugere ad gangen, mere end 10.000 modtagere pr. dag eller mere end 30 meddelelser pr. minut.
- Når du kører arbejdsgangen, sendes e-mailen ikke, og du bemærke følgende funktionsmåde:
    - For en arbejdsproces ved hjælp af typen SharePoint 2013-platform, kan du gå til **siden arbejdsprocesstatus** . På siden Status for arbejdsproces **Interne Status** er angivet til **startet**og markeringsboblen oplysninger viser **kunne ikke sendes til en modtager**.

Du kan løse dette problem ved at konfigurere arbejdsgangen til at sende e-mail-meddelelser uden at overskride [grænser for Exchange Online afsender](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Brug en pause i arbejdsprocessen, sende e-mailen til en Office 365-gruppe, en distributionsgruppe eller en sikkerhedsgruppe for post, der er aktiveret, eller send meddelelsen til mindre end 200 modtagere på én gang.


Du kan finde flere oplysninger i følgende [artikel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Relaterede emner
- [Oprette produktionsflow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint og Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 