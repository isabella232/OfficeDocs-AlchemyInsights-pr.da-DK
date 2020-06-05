---
title: Rettelse af Microsoft 365-apps Beklager, vi har midlertidig meddelelse om serverproblemer
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
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582697"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Rettelse af Microsoft 365-apps "Beklager, vi har midlertidige serverproblemer"

Hvis du modtager denne meddelelse, kan du prøve følgende:

1. Kontroller din firewall, dit antivirusprogram og dine proxyindstillinger for at bekræfte, at de ikke blokerer for internetadgang til Microsoft 365-apps. Se [URL-adresser og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Gå til **Start**  >  **kørsel**, og skriv derefter **services.msc**. Sørg for, at følgende tjenester alle kører:
    - Automatisk installation af netværksforbundne enheder
    - Tjenesten Netværksliste
    - Kendskab til netværksplacering
    - Windows-hændelseslog

Hvis en af disse tjenester ikke kører, kan du prøve at starte den. Hvis du har problemer med at starte tjenesten, skal du køre følgende kommando ved at åbne en kommandoprompt med udvidede tilladelser:

**sfc /scannow delte et**

Genstart computeren, når denne kommando er færdig.

Du kan finde detaljerede oplysninger under ["Vi kan desværre ikke oprette forbindelse til din konto. Prøv igen senere", når du aktiverer](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).