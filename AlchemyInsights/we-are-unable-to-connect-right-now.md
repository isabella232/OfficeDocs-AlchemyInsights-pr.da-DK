---
title: Aktiveringsproblem – Vi kan ikke oprette forbindelse lige nu
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
- "3408"
- "9001423"
ms.openlocfilehash: 5dad4b43efac2468b57351a4d6c96379ed505071ca144ec0aa518e975633bb18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998145"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Vi rettelse Microsoft 365 meddelelsen "Vi kan ikke oprette forbindelse lige nu"

Hvis du modtager denne meddelelse, kan du prøve følgende:

1. Kontrollér din firewall, din antivirussoftware og dine proxyindstillinger for at bekræfte, at de ikke blokerer internetadgang Microsoft 365 apps. Se [Microsofts URL-adresser og IP-adresseintervaller.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Gå til **Start**  >  **Kør**, og skriv **services.msc**. Sørg for, at følgende tjenester kører alle:
    - Automatisk konfiguration af netværksforbundne enheder
    - Netværklistetjeneste
    - Kendskab til netværksplacering
    - Windows Hændelseslog

Hvis en af disse tjenester ikke kører, kan du prøve at starte den. Hvis du har problemer med at starte tjenesten, skal du køre følgende kommando ved at åbne en kommandoprompt med administratorrettigheder:

**sfc /scannow**

Når denne kommando er fuldført, skal du genstarte computeren.

Du kan finde flere oplysninger [i "Vi beklager, men vi kan ikke oprette forbindelse til din konto. Du kan prøve igen senere", når du aktiverer Office fra Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).