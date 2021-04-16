---
title: Løs Bluetooth-problemer i Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001475"
- "3506"
ms.openlocfilehash: f20bf4a642e019c7901e988a027e0220f0f1b07b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812926"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a>Løs Bluetooth-problemer i Windows 10

Hvis ikonet Bluetooth mangler, eller Bluetooth ikke kan slås til eller fra, kan du køre Bluetooth-fejlfindingsværktøjet. [Åbn indstillingerne for fejlfinding](ms-settings:troubleshoot), klik på **Bluetooth** under Find og løs **andre problemer**, og klik på **Kør fejlfindingsværktøjet**.

Hvis du ikke kan se Bluetooth-ikonet, men Bluetooth vises i Enhedshåndtering:

1. Klik på Bluetooth i **Enhedshåndtering.** Tryk og hold (eller højreklik) på navnet på Bluetooth-adapteren, og klik på **Fjern enhed**.

2. Luk Windows-enheden, vent et par sekunder, og tænd den derefter igen. Windows forsøger at geninstallere driveren.

Hvis du for nylig har installeret Windows 10-opdateringer eller opgraderet til Windows 10, kan det være en ide at søge efter driveropdateringer:

1. I Enhedshåndtering skal du klikke **på Bluetooth** og derefter klikke på navnet på Bluetooth-adapteren (som kan indeholde ordet "radio").

2. Tryk og hold (eller højreklik) på Bluetooth-adapteren, og klik derefter på **Opdater**  >  **driversøgning automatisk efter opdateret driversoftware**. Følg trinnene, og klik derefter på **Luk**.

      - Hvis Windows ikke kan finde en ny Bluetooth-driver, skal du gå til pc-producentens websted og downloade den nyeste Bluetooth-driver derfra.

    - Når du har downloadet den, skal du klikke på Opdater **driver** Gennemse computeren efter driversoftware Søg efter den placering, hvor driverfilerne er gemt >  >    >   **OK**  >  **Næste,** og følg trinnene for at installere.

3. Når du har installeret den opdaterede driver, skal du genstarte computeren og derefter kontrollere, om det løser forbindelsesproblemet.

Hvis du vil have mere at vide om fejlfinding af Bluetooth-problemer, skal du se hele artiklen [Løs Bluetooth-problemer i Windows 10.](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems)
