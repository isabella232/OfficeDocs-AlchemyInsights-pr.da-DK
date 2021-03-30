---
title: Konfigurer indstillinger for beskyttelse af personlige oplysninger i Microsoft Edge
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
ms.openlocfilehash: 2367a7a55d1837fa7c7095fd0ac10ff1cf7ae72d
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404620"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a>Konfigurer indstillinger for beskyttelse af personlige oplysninger i Microsoft Edge

Hvis Microsoft Edge er installeret på ikke-Windows-platforme, sendes diagnostiske data og webstedsoplysninger som standard ikke til Microsoft. Men hvis Microsoft Edge er installeret på Windows 10, sendes diagnostiske data og webstedsoplysninger i overensstemmelse med brugernes indstillinger for [Diagnostiske Windows-data.](https://go.microsoft.com/fwlink/?linkid=2132472)

Hvis du vil konfigurere, hvordan Microsoft Edge håndterer dataindsamling for din organisation, skal du bruge følgende gruppepolitikker:
- [MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) aktiverer rapportering af brugs- og nedbrudsrelaterede data.
- [SendSiteInfoToImproveServices sender webstedsoplysninger,](https://go.microsoft.com/fwlink/?linkid=2132470) der bruges til at forbedre Microsoft-tjenester.

Du kan få mere at vide under [Konfigurer politikindstillinger.](https://go.microsoft.com/fwlink/?linkid=2132577)
