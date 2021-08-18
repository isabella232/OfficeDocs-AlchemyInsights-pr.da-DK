---
title: Konfigurer indstillinger for beskyttelse af personlige oplysninger Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 991f323249e15abd137c3e69b400e40503ed30dec6507cc5071a0b1af7f72bb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090292"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a>Konfigurer indstillinger for beskyttelse af personlige oplysninger Microsoft Edge

Hvis en Microsoft Edge installeret på ikke-Windows platforme, sendes diagnostiske data og webstedsoplysninger som standard ikke til Microsoft. Men hvis Microsoft Edge installeret på Windows 10, sendes diagnostiske data og webstedsoplysninger i henhold til Windows [indstillinger for diagnostiske data.](https://go.microsoft.com/fwlink/?linkid=2132472)

Hvis du vil konfigurere Microsoft Edge hvordan dataindsamling for organisationen skal håndteres, skal du bruge følgende gruppepolitikker:
- [MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) aktiverer rapportering af forbrugs- og nedbrudsrelaterede data.
- [SendSiteInfoToImproveServices sender webstedsoplysninger,](https://go.microsoft.com/fwlink/?linkid=2132470) der bruges til at forbedre Microsoft-tjenester.

Du kan få mere at vide under [Konfigurer politikindstillinger.](https://go.microsoft.com/fwlink/?linkid=2132577)
