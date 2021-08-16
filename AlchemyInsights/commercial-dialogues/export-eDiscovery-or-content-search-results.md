---
title: Eksportere resultater fra eDiscovery/indholdssøgning
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7221"
ms.openlocfilehash: de5d6f2bbf32ca1b7a0bbb9dd416fb19186d2e72ad57fbf25d9b55bd733fdc21
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988080"
---
# <a name="export-ediscoverycontent-search-results"></a>Eksportere resultater fra eDiscovery/indholdssøgning

Det kan være nødvendigt at eksportere søgeresultaterne til en PST-fil (fra mail) eller til oprindelige Office-dokumenter (fra SharePoint og OneDrive for Business websteder). Hvis det er ja, skal du gøre følgende:

- Sørg for, at din konto har fået de rette tilladelser til at eksportere. Du kan få mere at vide [under Tildel eDiscovery-tilladelse](https://go.microsoft.com/fwlink/?linkid=2102406).
- Sørg for, at computeren har opfyldt [alle krav.](https://docs.microsoft.com/office365/securitycompliance/export-search-results#before-you-begin) Ikke alle browsere understøttes, f.eks. Chrome.
- Sådan eksporteres fra en Indholdssøgning: a. Gå til Security [& Compliance Center,](https://protection.office.com/contentsearch) og klik **på Søg**, og vælg derefter **Indholdssøgning**. Vælg en **gemt søgning** på siden Indholdssøgning.
    b. I ruden Detaljer under **Eksportér resultater til en computer skal** du vælge Start **eksport.** Hvis du eksporterer mere end 100.000 postkasser, skal du bruge PowerShell til at hente eksportresultaterne. Få mere at vide under [Eksport af resultater fra mere end 100.000 postkasser.](https://go.microsoft.com/fwlink/?linkid=2143861)

Du kan få mere at vide [under Eksportér resultater fra indholdssøgning.](https://go.microsoft.com/fwlink/?linkid=2102118)