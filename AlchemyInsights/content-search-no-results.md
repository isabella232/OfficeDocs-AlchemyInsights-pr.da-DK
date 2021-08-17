---
title: Indholdssøgning uden resultater
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
- "9000661"
- "2527"
ms.openlocfilehash: b53534dd0666fa64e692910aa6800abab30169a97fbe567c815ce6b948381a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057996"
---
# <a name="no-results-from-content-searchexports"></a>Ingen resultater fra indholdssøgning/eksporter

Problemer med indholdssøgning/eksporter, der ikke returnerer nogen data, kan skyldes et bestemt sikkerhedsfilter til overholdelse, der er konfigureret af en bestemt administrator og ikke kommunikerer det til alle administratorer.

For at løse dette skal du kontrollere, om der er nogen sikkerhedsfiltre til overholdelse af regler og standarder, der kan være skyld i dette:
1. Forbind til Security and Compliance Center Powershell
2. Kør følgende kommandoletter:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter – $org