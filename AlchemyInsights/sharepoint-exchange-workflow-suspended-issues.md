---
title: Introduktion til SharePoint Online
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: 5e61491b626bfe75fd26a15ee54be82d9efa19a7
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 11/15/2019
ms.locfileid: "37766885"
---
# <a name="workflows-in-sharepoint"></a>Arbejdsprocesser i SharePoint

Hvis SharePoint-arbejdsprocesser ikke sender mails, kan din organisation være stødt på grænserne for afsenderens Exchange Online-afsender.

Fejlmeddelelsen ' arbejdsprocessen er suspenderet ' kan opstå, hvis du har et af følgende elementer:

- Du har en arbejdsproces i SharePoint Online, der bruger SharePoint 2010-eller SharePoint 2013-arbejdsgangs platforms typen.

- Arbejdsprocessen er konfigureret til at sende en brugerdefineret e-mail-meddelelse til mere end 200 brugere ad gangen, mere end 10.000 modtagere pr. dag eller mere end 30 meddelelser pr. minut.

Når du kører arbejdsprocessen, sendes e-mailen ikke, og du bemærker fejlmeddelelsen, den interne status er indstillet til suspenderet eller ikke kan sendes til en modtager vises.

Yderligere oplysninger finder du i følgende [artikel](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).

