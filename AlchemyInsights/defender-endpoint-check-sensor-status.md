---
title: Defender Endpoint kontrollerer sensorens status
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676099"
---
# <a name="defender-endpoint-check-sensor-status"></a>Defender Endpoint kontrollerer sensorens status

Feltet **Enheder med sensorproblemer** findes på dashboardet Sikkerhedshandlinger. Dette felt indeholder oplysninger om den enkelte enheds mulighed for at levere sensordata og kommunikere med Defender for Endpoint-tjenesten. Den rapporterer, hvor mange enheder der kræver opmærksomhed, og hjælper dig med at identificere problematiske enheder og tage skridt til at rette kendte problemer.

To statusindikatorer på feltet indeholder oplysninger om antallet af enheder, der ikke rapporterer korrekt til tjenesten:

- **Forkert konfigureret** Enheder, der muligvis delvist rapporterer sensordata til Defender for Endpoint-tjenesten, og som muligvis har konfigurationsfejl, der skal rettes.
- **Inaktiv** Enheder, der er holdt op med at rapportere til Defender for Endpoint-tjenesten i mere end syv dage i den sidste måned.

Når du klikker på en af grupperne, dirigeres du til listen Enheder, der er filtreret efter dine valg. På listen Enheder kan du filtrere listen over tilstandstilstande ud fra følgende status:

- **Aktiv** Enheder, der aktivt rapporterer til Defender for Endpoint-tjenesten.
- **Forkert konfigureret** Enheder, der muligvis delvist rapporterer sensordata til Defender for Endpoint-tjenesten, men har konfigurationsfejl, der skal rettes. Forkert konfigurerede enheder kan have enten en eller en kombination af følgende problemer:

    - Ingen sensordata – Enheder er holdt op med at sende sensordata. Der kan udløses begrænsede beskeder fra enheden.
    - Forringet kommunikation – Muligheden for at kommunikere med enheden er forringet. Det fungerer muligvis ikke at sende filer til dybdegående analyse, blokere filer, isolere enheden fra netværket og andre handlinger, der kræver kommunikation med enheden.
- **Inaktiv** Enheder, der er holdt op med at rapportere til Defender for Endpoint-tjenesten.

Du kan downloade hele listen i CSV-format ved hjælp af funktionen Eksportér.

Du kan få mere at vide [under Kontrollér tilstanden for sensorens tilstand i Microsoft Defender til slutpunkt](/microsoft-365/security/defender-endpoint/check-sensor-status).

Du kan finde flere oplysninger om, hvad der forårsagede, at en enhed var inaktiv eller forkert konfigureret, under Ret [usunde sensorer i Microsoft Defender til slutpunkt.](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)
