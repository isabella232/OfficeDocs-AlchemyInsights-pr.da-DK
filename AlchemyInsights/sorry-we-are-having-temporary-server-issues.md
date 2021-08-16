---
title: Vi beklager Microsoft 365, men vi har midlertidige serverproblemer
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
- "3420"
- "9001430"
ms.openlocfilehash: aa0d625856df1027146de5af57845224e3056d8c21d9ac4cefbd4a9c329f487c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54021590"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Vi rettelse Microsoft 365 fejlmeddelelsen "Vi beklager, men vi har midlertidige serverproblemer"

Hvis du modtager denne meddelelse, kan du prøve følgende:

1. Kontrollér din firewall, din antivirussoftware og dine proxyindstillinger for at bekræfte, at de ikke blokerer internetadgang Microsoft 365 apps. Se [URL-adresser og IP-adresseintervaller](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Gå til **Start**  >  **Kør**, og skriv **services.msc**. Sørg for, at følgende tjenester kører alle:
    - Automatisk konfiguration af netværksforbundne enheder
    - Netværklistetjeneste
    - Kendskab til netværksplacering
    - Windows Hændelseslog

Hvis en af disse tjenester ikke kører, kan du prøve at starte den. Hvis du har problemer med at starte tjenesten, skal du køre følgende kommando ved at åbne en kommandoprompt med administratorrettigheder:

**sfc /scannow**

Når denne kommando er fuldført, skal du genstarte computeren.

Du kan finde flere oplysninger [i "Vi beklager, men vi kan ikke oprette forbindelse til din konto. Prøv igen senere"-fejlen, når du aktiverer](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).