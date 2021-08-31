---
title: Vi beklager Microsoft 365 der er problemer med midlertidige serverproblemer i forbindelse med apps
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
ms.openlocfilehash: 565f70d9a09c61bef84cdd1c23e9b0ed34bebe51
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744640"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Vi rettelse Microsoft 365 fejlmeddelelsen "Vi beklager, men vi har midlertidige serverproblemer"

Bemærk! Hvis du bruger en ældre version af Windows (f.eks. Windows 7 SP1, Windows Server 2008 R2), skal du bruge den nemme løsning til at aktivere TLS 1.2 som standard. [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) Få mere at vide under Opdater for at aktivere [TLS 1.1 og TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)som standard sikre protokoller i WinHTTP Windows .

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