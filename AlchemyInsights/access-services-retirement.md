---
title: Adgangstjenester pensionering
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: cb8123583b68e945ef878fdbaf211fd1d8205bb3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050483"
---
# <a name="access-services-retirement"></a>Adgangstjenester pensionering

Som vi oprindeligt annonceret i MC97576, i marts 2017, og fortsatte med at kommunikere i løbet af det seneste år adgangstjenester er ved at blive pensioneret fra Office 365. Den næste fase i denne proces vil være fjernelsen af Access-webdatabaser, der bruger SharePoint-lister som deres underliggende datalager.

**Hvordan påvirker det mig?**

Fra og med juni 2019 vil vi stoppe oprettelsen af nye Access-databaser i SharePoint Online og lukke tjenesten og eventuelle resterende apps senest i april 2020.

**Hvad skal jeg gøre for at forberede mig på denne ændring?**

Vi opfordrer dig til at oprette en overgangsplan for organisationens Access-webdatabaser. Administratorer kan bruge [SharePoint Access-appscanneren](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) til at hente en oversigt med de Access-apps, som websteder bruger.

Der er flere måder at migrere Access web databases data:

- Importerer til en lokal Access-database (. ACCDB) eller til en Excel-fil.
- Vi anbefaler også, at du udforsker Microsoft PowerApps som en alternativ platform til at oprette forretningsløsninger uden kode til web-og mobilenheder.