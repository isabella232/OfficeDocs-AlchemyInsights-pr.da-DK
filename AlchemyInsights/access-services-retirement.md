---
title: Adgang tjenester pensionering
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
ms.openlocfilehash: 977bd5887ef58b328463a9befcd6b47ac55f5a85
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687252"
---
# <a name="access-services-retirement"></a>Adgang tjenester pensionering

Som vi oprindeligt annonceret i MC97576, i marts 2017, og fortsatte med at kommunikere i det forløbne år Access Services bliver pensioneret. Den næste fase i denne proces vil være fjernelse af Access Web-databaser, der bruger SharePoint lister som deres underliggende datalagring.

**Hvordan påvirker det mig?**

Fra juni 2019 stopper vi oprettelsen af nye Access-databaser i SharePoint Online og lukker tjenesten og eventuelle resterende apps inden april 2020.

**Hvad skal jeg gøre for at forberede mig på denne ændring?**

Vi opfordrer dig til at oprette en overgangsplan for organisationens Access-webdatabaser. Administratorer kan bruge [SharePoint Access-appscanneren](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) til at få en oversigt over de Access-apps, som websteder bruger.

Du kan overføre Data til Access-webdatabaser på flere måder:

- Import til en lokal Access-database (. ACCDB) eller til en Excel-fil.
- Vi anbefaler også, at du udforsker Microsoft PowerApps som en alternativ platform til at oprette forretningsløsninger uden kode til web- og mobilenheder.