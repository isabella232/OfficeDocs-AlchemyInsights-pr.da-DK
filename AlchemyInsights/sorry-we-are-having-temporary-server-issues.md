---
title: Rettelse af Microsoft 365-apps vi beklager, men vi har midlertidige serverproblemer-meddelelse
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
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758239"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Hvis du retter Microsoft 365-apps, kan vi desværre ikke få besked om midlertidige serverproblemer

Hvis du får vist denne meddelelse, kan du prøve følgende:

1. Kontrollér din firewall, antivirussoftware og proxyindstillinger for at bekræfte, at de ikke blokerer Internet adgang til Microsoft 365-apps. Se [URL-adresser og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Gå til **Start**  >  **Run**, og Skriv **Services. msc**. Sørg for, at følgende tjenester alle kører:
    - Automatisk konfiguration af netværksforbundne enheder
    - Netværksliste tjeneste
    - Netværks placerings bevidsthed
    - Logbog i Windows

Hvis en af disse tjenester ikke kører, skal du prøve at starte det. Hvis du har problemer med at starte tjenesten, skal du køre følgende kommando ved at åbne en kommandoprompt med administratorrettigheder:

**sfc/scannow**

Genstart computeren, når denne kommando er færdig.

Hvis du vil have mere at vide, skal du se ["beklager, vi kan ikke oprette forbindelse til din konto. Prøv igen senere "-fejl, når du aktiverer](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).