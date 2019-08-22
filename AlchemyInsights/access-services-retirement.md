---
title: Access services-pension
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 8886d7a6fad49e942e17f6a2f3c98542f87aae0b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36495745"
---
# <a name="access-services-retirement"></a>Access services-pension

Da vi oprindeligt blev offentliggjort i MC97576, i marts 2017 og fortsatte med at kommunikere over det seneste år er Access Services bliver afbrudt fra Office 365. Den næste fase i denne proces vil være fjernelse af Web Access-databaser, der bruger SharePoint-lister som deres underliggende datalager.

**Hvordan påvirker det mig?**

Start juni 2019, vi stopper oprettelsen af nye Access-databaser i SharePoint Online og lukke tjenesten og eventuelle resterende apps ved April 2020.

**Hvad skal jeg gøre for at forberede denne ændring?**

Vi opfordrer dig til at oprette en plan for overgangen til organisationens Access web-databaser. Administratorer kan bruge [SharePoint adgang app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) til at få en oversigt over Access-programmer, websteder bruger.

Der er flere måder at overføre data fra Access web databaser:

- Import til en lokal database i Access (. ACCDB) eller en Excel-fil.
- Vi anbefaler også, at udforske Microsoft PowerApps som en alternativ platform til at oprette uden kode forretningsløsninger til web og mobile enheder.