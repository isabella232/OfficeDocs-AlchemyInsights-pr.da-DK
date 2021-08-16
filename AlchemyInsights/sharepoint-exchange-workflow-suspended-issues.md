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
ms.openlocfilehash: a14705003f742641f10c8459b7c7024146e4134a8d5113451e5732cef7326484
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54051408"
---
# <a name="workflows-in-sharepoint"></a>Arbejdsprocesser i SharePoint

Hvis SharePoint arbejdsprocesser ikke sender mails, kan din organisation have oplevet de Exchange Online afsenderbegrænsninger.

Fejlmeddelelsen "Arbejdsprocessen er afbrudt" kan opstå, hvis du har et af følgende elementer:

- Du har en arbejdsproces i SharePoint Online, der bruger SharePoint 2010 eller SharePoint 2013-arbejdsprocesplatformtypen.

- Arbejdsprocessen er konfigureret til at sende en brugerdefineret mail til mere end 200 brugere ad gangen, mere end 10.000 modtagere pr. dag eller mere end 30 meddelelser i minuttet.

Når du kører arbejdsprocessen, sendes mailen ikke, og du bemærker fejlmeddelelsen Intern status er angivet til Afbrudt eller Kan ikke sende til en modtager vises.

Du kan finde flere oplysninger i følgende [artikel.](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running)

