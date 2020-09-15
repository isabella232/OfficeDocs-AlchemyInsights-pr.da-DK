---
title: Dynamics 365-forkert Dashboard vises i Dynamics 365 Unified interface
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711269"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Forkert Dashboard vises i Dynamics 365 Unified interface

Der er flere årsager til, at du kan se et andet dashboard, end det, du forventer:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Brugeren har konfigureret et brugerdefineret Dashboard 

Du kan typisk identificere et bruger standarddashboard, hvis knappen **Angiv som standard** ikke vises på Dashboard kommandolinjen. Standard dashboardet for brugeren tilsidesætter alle andre standarddashboards, også selvom brugerens standarddashboard ikke er i den aktuelle app.

Brug følgende løsning til at fjerne standard dashboardet.

1. Opret et nyt personligt Dashboard.

2. Angiv det nye Dashboard som bruger standard.

3. Slet dette Dashboard.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Dashboardet er angivet i sitemap

Du har muligvis angivet et dashboard for organisationen ved at vælge et dashboard og vælge "Angiv som standard" under ' Tilpas systemet '. Men det Dashboard, der er defineret i sitemap designer, tilsidesætter dette Dashboard, hvis brugeren har adgang til det.

Hvis du vil have brugerne til at se det Dashboard, du har angivet som organisations standard, kan du enten:

* Indstille dette Dashboard i sitemap

* Fjernadgang til det sitemap-Dashboard, der er defineret for disse brugere
