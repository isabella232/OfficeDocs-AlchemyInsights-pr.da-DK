---
title: Ret Bluetooth-problemer i Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001475"
- "3506"
ms.openlocfilehash: 7e7a397a1f6777972a81bcbb6bffa1c98d8370a4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730153"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a>Ret Bluetooth-problemer i Windows 10

Hvis Bluetooth-ikonet mangler, eller Bluetooth ikke kan slås til eller fra, kan det være en god ide at køre Bluetooth-fejlfinding. [Åbn fejlfindingsindstillinger](ms-settings:troubleshoot), klik på **Bluetooth** under **Søg og løs andre problemer**, og klik på **Kør fejlfindingsværktøjet**.

Hvis du ikke kan se Bluetooth-ikonet, men Bluetooth vises i Enhedshåndtering:

1. Klik på **Bluetooth**i Enhedshåndtering. Tryk på og hold (eller højreklik) på Bluetooth-kortets navn, og klik på **Fjern enhed**.

2. Luk din Windows-enhed, vent et øjeblik, og tænd for det igen. Windows vil forsøge at geninstallere driveren.

Hvis du for nylig har installeret Windows 10-opdateringer eller opgraderet til Windows 10, kan du kontrollere, om der er driveropdateringer:

1. I Enhedshåndtering skal du klikke på **Bluetooth**og derefter klikke på navnet på Bluetooth-kortet (som muligvis indeholder ordet "radio").

2. Tryk på og hold (eller højreklik) på Bluetooth-adapteren, og klik derefter på **Opdater driver**  >  **søgning automatisk for at få opdateret driversoftware**. Følg trinnene, og klik derefter på **Luk**.

      - Hvis Windows ikke kan finde en ny Bluetooth-driver, skal du gå til PC-producentens websted og hente den nyeste Bluetooth-driver derfra.

    - Når du har hentet det, skal du klikke på **Opdater driver**  >  **Gennemse min computer for driversoftware**  >  **Find** den placering, hvor driverfilerne er gemt > **OK**  >  **næste**, og følg trinnene for at installere.

3. Når du har installeret den opdaterede driver, skal du genstarte computeren og derefter kontrollere, om det løser forbindelsesproblemet.

Du kan finde flere oplysninger om, hvordan du foretager fejlfinding af Bluetooth-problemer, i hele artiklen, [rette Bluetooth-problemer i Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).
