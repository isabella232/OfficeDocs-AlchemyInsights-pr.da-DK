---
title: Brug sikkerhedsplaner for Microsoft Intune til at konfigurere Windows 10-enheder
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573331"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Brug sikkerhedsplaner for Microsoft Intune til at konfigurere Windows 10-enheder

Intune-sikkerhedsplaner hjælper med at beskytte brugere og enheder. Sikkerhedsplaner er Windows-indstillinger ' forudkonfigurerede grupper, der bruges til at anvende en kendt gruppe af indstillinger og standardværdier, der anbefales af de relevante sikkerheds teams. Hvis du opretter en oprindelig plan for oprindelige profiler i Intune, opretter du en skabelon, der består af flere enheds konfigurationsprofiler.

Når du installerer sikkerhedsplaner til grupper af brugere eller enheder, anvendes indstillingerne på enheder, der kører på Windows 10 eller nyere. For eksempel gør MDM-sikkerheds grundlinje automatisk (1) aktiverer BitLocker for flytbare drev, (2) kræver adgangskoden til at låse en enhed op, og (3) deaktiverer grundlæggende godkendelse. Når en standardværdi ikke fungerer for dit miljø, kan du tilpasse grundlinjen for at anvende de ønskede indstillinger.

Sikkerhedsplaner hjælper også med at oprette en slut-til-slut-arbejdsproces i Microsoft 365. Følgende er nogle fordele ved dette:

- En sikkerheds basis omfatter de bedste fremgangsmåder og anbefalinger til indstillinger, der påvirker sikkerheden. Da Intune-partnere med Windows-sikkerheds teamet, der opretter grundlinjer til gruppepolitikker, er disse anbefalinger baseret på en dækkende vejledning og en omfattende oplevelse.
- Hvis du er ny bruger af Intune og ikke er sikker på, hvor du skal starte, kan du bruge sikkerhedsplaner til hurtigt at oprette og installere en sikker profil.
- Hvis du i øjeblikket bruger en gruppepolitik, er det meget nemmere at overføre til Intune til administrationsformål, fordi de er indbygget i Intune og omfatter de allernyeste funktioner til administration.

Hvis du vil have mere at vide, skal du se [Windows-sikkerhedsplaner](https://go.microsoft.com/fwlink/?linkid=2141503) og [administration af mobilenheder](https://go.microsoft.com/fwlink/?linkid=2141701).