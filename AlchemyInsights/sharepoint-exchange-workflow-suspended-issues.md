---
title: Introduktion til SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: bba89489cb75555e1f508224de223bee04e1d665
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700701"
---
# <a name="workflows-in-sharepoint"></a>Arbejdsprocesser i SharePoint

Hvis SharePoint-arbejdsprocesser ikke sender mails, kan din organisation have registreret Exchange Online-afsender grænsen.

Fejlmeddelelsen "arbejdsprocessen er suspenderet" kan forekomme, hvis du har et af følgende elementer:

- Du har en arbejdsproces i SharePoint Online, der bruger SharePoint 2010-eller SharePoint 2013-typen arbejdsproces platform.

- Arbejdsprocessen er konfigureret til at sende en brugerdefineret mail til mere end 200 brugere ad gangen, mere end 10.000 modtagere pr. dag eller mere end 30 meddelelser pr. minut.

Når du kører arbejdsprocessen, bliver mail meddelelsen ikke sendt, og du bemærker fejlmeddelelsen, den interne status er sat til suspenderet eller kan ikke sendes til en modtager vises.

Hvis du vil have mere at vide, skal du se følgende [artikel](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).

