---
title: Aktiveringsproblem - Vi kan ikke oprette forbindelse lige nu
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
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716166"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a>Rettelse af Office-apps "Vi kan ikke oprette forbindelse lige nu"

Hvis du modtager denne meddelelse, kan du prøve følgende:

1. Kontroller dine firewall-, antivirusprogrammer s- og proxyindstillinger for at bekræfte, at de ikke blokerer for internetadgang til Office-apps. Se [MicrosoftURL-adresser og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Gå til **Start** > **kørsel**, og skriv derefter **services.msc**. Sørg for, at følgende tjenester kører:
    - Automatisk installation af netværksforbundne enheder
    - Tjenesten Netværksliste
    - Kendskab til netværksplacering
    - Windows-hændelseslog

Hvis en af disse tjenester ikke kører, kan du prøve at starte den. Hvis du har problemer med at starte tjenesten, skal du køre følgende kommando ved at åbne en kommandoprompt med udvidede tilladelser:

**sfc /scannow**

Når kommandoen er færdig, skal du genstarte computeren.

Du kan finde detaljerede oplysninger under ["Vi kan desværre ikke oprette forbindelse til din konto. Prøv igen senere", når du aktiverer Office fra Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).