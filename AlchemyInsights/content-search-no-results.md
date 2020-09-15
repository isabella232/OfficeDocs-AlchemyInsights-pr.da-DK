---
title: Indholdssøgning uden resultater
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
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680641"
---
# <a name="no-results-from-content-searchexports"></a>Ingen resultater fra indholdssøgning/eksport

Problemer med indholdssøgning/eksport, der ikke returnerer nogen data, kan skyldes et bestemt sikkerheds filter for overholdelse, der blev konfigureret af en bestemt administrator og ikke kommunikerer med alle administratorer.

Hvis du vil løse dette, skal du kontrollere, om der er nogen sikkerhedsfiltre overholdelse, der kan forårsage dette:
1. Opret forbindelse til sikkerheds-og overholdelses Center PowerShell
2. Kør følgende commandlets:
<br>$org = "yourdomain.com"
<br>Få ComplianceSecurityFilter-organisation $org