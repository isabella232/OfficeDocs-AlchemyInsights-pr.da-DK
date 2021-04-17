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
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816842"
---
# <a name="no-results-from-content-searchexports"></a>Ingen resultater fra indholdssøgning/eksporter

Problemer med indholdssøgning/eksporter, der ikke returnerer nogen data, kan skyldes et bestemt sikkerhedsfilter til overholdelse, der er konfigureret af en bestemt administrator og ikke kommunikerer det til alle administratorer.

For at løse dette skal du kontrollere, om der er nogen sikkerhedsfiltre til overholdelse af regler og standarder, der kan være skyld i dette:
1. Opret forbindelse til Security and Compliance Center Powershell
2. Kør følgende kommandoletter:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter – $org