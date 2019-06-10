---
title: Access services-pension
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: f5a1e88e4443fdf43cdd4f07cf9e784810df7540
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/07/2019
ms.locfileid: "34769431"
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