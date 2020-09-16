---
title: Aktiverings problem-vi kan ikke oprette forbindelse lige nu
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
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725977"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Retter Microsoft 365-apps "vi kan ikke oprette forbindelse lige nu"

Hvis du får vist denne meddelelse, kan du prøve følgende:

1. Kontrollér din firewall, antivirussoftware og proxyindstillinger for at bekræfte, at de ikke blokerer Internet adgang til Microsoft 365-apps. Se [Microsoft URL-adresser og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Gå til **Start**  >  **Run**, og Skriv **Services. msc**. Sørg for, at følgende tjenester alle kører:
    - Automatisk konfiguration af netværksforbundne enheder
    - Netværksliste tjeneste
    - Netværks placerings bevidsthed
    - Logbog i Windows

Hvis en af disse tjenester ikke kører, skal du prøve at starte det. Hvis du har problemer med at starte tjenesten, skal du køre følgende kommando ved at åbne en kommandoprompt med administratorrettigheder:

**sfc/scannow**

Genstart computeren, når denne kommando er færdig.

Hvis du vil have mere at vide, skal du se ["beklager, vi kan ikke oprette forbindelse til din konto. Prøv igen senere "-fejl, når du aktiverer Office fra Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).