---
title: Adgangstjenester pensionering
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 197366882468ebc87fc26f2fe2733371790d1871
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/04/2019
ms.locfileid: "36747778"
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