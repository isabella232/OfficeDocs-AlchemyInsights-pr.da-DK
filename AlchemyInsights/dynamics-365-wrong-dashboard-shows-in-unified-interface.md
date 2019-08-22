---
title: Dynamics 365 - forkert Dashboard viser i Dynamics 365 Unified grænseflade
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36528545"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Forkert dashboard viser i Dynamics 365 unified grænseflade

Der er flere grunde, hvorfor du kan se et andet dashboard end den, du forventer:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Brugeren har angivet et brugerdashboard standard 

Typisk kan du identificere en bruger standarddashboard angives, hvis knappen **Vælg som standard** ikke vises på dashboard-kommandolinjen. Standard brugerdashboard tilsidesætter alle andre standard dashboards, selvom brugerens standarddashboard ikke er i den aktuelle app.

Brug følgende fremgangsmåde til at fjerne deres standarddashboard.

1. Opret et nyt personligt instrumentbræt.

2. Angiv den nye dashboard som standard bruger.

3. Slet dette dashboard.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Dashboardet er angivet i sitemap

Du kan angive et standarddashboard for organisationen ved at vælge et dashboard og vælge 'Angiv som standard' under 'Tilpasse systemet'. Men det dashboard, der er defineret i sitemap designer højere prioritet end dette dashboard, hvis brugeren har adgang til den.

Hvis brugerne kan se det dashboard, du har angivet som standard organisation, kan du enten:

* Angiv dette dashboard i sitemap

* Fjern adgang til dashboardet sitemap, der er defineret for disse brugere
