---
title: Løsning af Office-apps Beklager, vi har midlertidige serverproblemer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764111"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>Rettelse af Office-apps "Beklager, vi har midlertidige serverproblemer"

Hvis du modtager denne meddelelse, kan du prøve følgende:

1. Kontroller dine firewall-, antivirusprogrammer s- og proxyindstillinger for at bekræfte, at de ikke blokerer for internetadgang til Office-apps. Se [URL-adresser og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Gå til **Start** > **kørsel**, og skriv derefter **services.msc**. Sørg for, at følgende tjenester kører:
    - Automatisk installation af netværksforbundne enheder
    - Tjenesten Netværksliste
    - Kendskab til netværksplacering
    - Windows-hændelseslog

Hvis en af disse tjenester ikke kører, kan du prøve at starte den. Hvis du har problemer med at starte tjenesten, skal du køre følgende kommando ved at åbne en kommandoprompt med udvidede tilladelser:

**sfc /scannow**

Når kommandoen er færdig, skal du genstarte computeren.

Du kan finde detaljerede oplysninger under ["Vi kan desværre ikke oprette forbindelse til din konto. Prøv igen senere",, når du aktiverer](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).