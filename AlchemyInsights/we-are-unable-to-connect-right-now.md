---
title: Aktiverings problem-vi kan ikke oprette forbindelse lige nu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 84e3a7700558ad8a5fad5b7ded6354fe8736e0f7
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628236"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a>Rettelse af Office-Apps "vi kan ikke oprette forbindelse lige nu"-meddelelse

Hvis du modtager denne meddelelse, kan du prøve følgende:

1. Kontrollér din firewall, dit antivirusprogram og dine proxyindstillinger for at bekræfte, at de ikke blokerer for Internet adgang til Office-Apps. Se [Office 365 URL-adresser og IP-adresse intervaller](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Gå til **Start** > **Kør**, og skriv derefter **Services. msc**. Sørg for, at følgende tjenester alle kører:
    - Automatisk konfiguration af netværkstilsluttede enheder
    - Tjenesten netværksliste
    - Kendskab til netværksplacering
    - Windows hændelseslog

Hvis en af disse tjenester ikke kører, kan du prøve at starte den. Hvis du har problemer med at starte tjenesten, skal du køre følgende kommando ved at åbne en kommandoprompt med administratorrettigheder:

**sfc/scannow**

Når denne kommando er færdig, skal du genstarte computeren.

Yderligere oplysninger finder du under ["beklager, vi kan ikke oprette forbindelse til din konto. Prøv igen senere ", når du aktiverer Office fra Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).