---
title: Dynamics 365-forkerte Dashboard-programmer i Dynamics 365 Unified interface
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/25/2019
ms.locfileid: "36528545"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Forkerte Dashboard-shows i Dynamics 365 Unified interface

Der er flere grunde til, at du kan se et andet dashboard end det, du forventer:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Brugeren har angivet et bruger standarddashboard 

Typisk kan du identificere et bruger standarddashboard er indstillet, hvis knappen **Angiv som standard** ikke vises på Dashboard kommandolinjen. Bruger standarddashboardet tilsidesætter alle andre standarddashboards, selvom brugerens standarddashboard ikke findes i den aktuelle app.

Brug følgende løsning til at fjerne et standarddashboard.

1. Opret et nyt personligt Dashboard.

2. Angiv det nye Dashboard som bruger standard.

3. Slet dashboardet.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Dashboardet er angivet i sitemap

Du har måske indstillet et organisations standarddashboard ved at vælge et dashboard og vælge ' Angiv som standard ' under ' Tilpas systemet '. Men dashboardet, der er defineret i sitemap-designeren, har forrang for dette Dashboard, hvis brugeren har adgang til det.

Hvis brugerne skal kunne se det Dashboard, du har angivet som organisationens standard, kan du enten:

* Indstil dashboardet i sitemap

* Fjernadgang til det sitemap-definerede Dashboard for disse brugere
