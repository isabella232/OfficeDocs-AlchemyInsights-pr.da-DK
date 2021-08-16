---
title: Dynamics 365 – Forkert dashboard viser i Dynamics 365 Unified Interface
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
ms.openlocfilehash: 1edb2a7e9e0c270c7e98eb43d2f6514d70c39a19ea97d189322ca387b6842a18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101476"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Forkert dashboard vises i den samlede Dynamics 365-grænseflade

Der er flere årsager til, at du kan få vist et andet dashboard end det, du forventer:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Brugeren har angivet et standarddashboard for brugeren 

Du kan typisk identificere, at et  standarddashboard er angivet, hvis knappen Angiv som standard ikke vises på dashboardkommandolinjen. Brugerens standarddashboard tilsidesætter alle andre standarddashboards, også selvom brugerens standarddashboard ikke er i den aktuelle app.

Brug følgende løsning til at fjerne deres standarddashboard.

1. Opret et nyt personligt dashboard.

2. Angiv det nye dashboard som standard for brugeren.

3. Slet dashboardet.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Dashboardet er angivet i webstedsoversigten

Du kan have indstillet en organisations standarddashboard ved at vælge et dashboard og vælge "Angiv som standard" under "Tilpas systemet". Men det dashboard, der er defineret i webstedsoversigtdesigneren, tilsidesætter dette dashboard, hvis brugeren har adgang til det.

For at få brugerne til at se det dashboard, du har angivet som organisationens standard, kan du enten:

* Angiv dashboardet i webstedsoversigten

* Fjern adgang til det webstedsoversigtsdefinerede dashboard for disse brugere
