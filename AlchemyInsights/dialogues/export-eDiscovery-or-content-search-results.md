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
ms.openlocfilehash: b93377a33eebc7899041b684449e46caedb04415
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429412"
---
# <a name="export-ediscoverycontent-search-results"></a>Eksportere resultater fra eDiscovery/indholdssøgning

Det kan være nødvendigt at eksportere søgeresultaterne til en PST-fil (fra mail) eller til oprindelige Office-dokumenter (fra SharePoint- og OneDrive for Business-websteder). Hvis det er nødvendigt, skal du gøre følgende:

- Sørg for, at din konto er tildelt de rette tilladelser til at eksportere. Du kan finde flere oplysninger under [Tildel eDiscovery-tilladelse.](https://go.microsoft.com/fwlink/?linkid=2102406)
- Sørg for, at computeren har opfyldt [alle forudsætningerne.](https://docs.microsoft.com/office365/securitycompliance/export-search-results#before-you-begin) Ikke alle browsere understøttes, f.eks. Chrome.
- Sådan eksporteres fra en indholdssøgning: a. Gå til [Sikkerheds- &, og](https://protection.office.com/contentsearch) klik på **Søg,** og vælg derefter **Indholdssøgning.** Vælg en **gemt søgning** på siden Indholdssøgning.
    b. Vælg **Start** eksport i detaljeruden under **Eksportér resultater** til en computer. Hvis du eksporterer mere end 100.000 postkasser, skal du bruge PowerShell til at hente eksportresultaterne. Du kan finde flere oplysninger i [Eksportere resultater fra mere end 100.000 postkasser.](https://go.microsoft.com/fwlink/?linkid=2143861)

Du kan få mere at vide under [Eksportér søgeresultater for indhold.](https://go.microsoft.com/fwlink/?linkid=2102118)