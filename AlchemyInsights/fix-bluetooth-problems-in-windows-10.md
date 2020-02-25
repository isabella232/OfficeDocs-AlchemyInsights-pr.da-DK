---
title: Løs Bluetooth-problemer i Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001475"
- "3506"
ms.openlocfilehash: 94dda7a42632f57ce3aef5f467b87df1033b8d49
ms.sourcegitcommit: 9a35768444824cde9e192f1d9daafc9157437244
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/25/2020
ms.locfileid: "42268592"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a>Løs Bluetooth-problemer i Windows 10

Hvis Bluetooth-ikonet mangler, eller Bluetooth ikke kan tændes eller slukkes, kan det være en god ide at køre Bluetooth-fejlfindingsværktøjet. [Åbn indstillingerne for fejlfinding](ms-settings:troubleshoot), klik på **Bluetooth** under Søg og løs **andre problemer**, klik på **Kør fejlfindingsværktøjet**.

Hvis du ikke kan se Bluetooth-ikonet, men Bluetooth vises i Enhedshåndtering:

1. Klik på **Bluetooth**i Enhedshåndtering. Tryk og hold (eller højreklik) på Bluetooth-kortnavnet, og klik på **Fjern enhed**.

2. Luk windows-enheden, vent et par sekunder, og tænd den derefter igen. Windows forsøger at geninstallere driveren.

Hvis du for nylig har installeret Windows 10-opdateringer eller opgraderet til Windows 10, kan det være en god ide at søge efter driveropdateringer:

1. Klik på **Bluetooth**i Enhedshåndtering, og klik derefter på Navnet på Bluetooth-adapteren (som kan indeholde ordet "radio").

2. Tryk og hold (eller højreklik) på Bluetooth-kortet, og klik derefter på **Opdater driversøgning** > **automatisk efter opdateret driversoftware**. Følg trinnene, og klik derefter på **Luk**.

      - Hvis Windows ikke kan finde en ny Bluetooth-driver, kan du besøge pc-producentens websted og hente den nyeste Bluetooth-driver derfra.

    - Når du har hentet den, skal du klikke på **Opdater driver** > **Gennemse min computer efter driversoftware** > **Søg efter** det sted, hvor driverfilerne er gemt > **OK** > **Næste**, og følg trinnene for at installere.

3. Når du har installeret den opdaterede driver, skal du genstarte computeren og derefter kontrollere, om det løser forbindelsesproblemet.

Yderligere oplysninger om fejlfinding af Bluetooth-problemer finder du i hele [artiklen, Løs Bluetooth-problemer i Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).
