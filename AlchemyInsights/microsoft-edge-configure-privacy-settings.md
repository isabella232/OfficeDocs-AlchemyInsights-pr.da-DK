---
title: Microsoft Edge konfigurere indstillinger for beskyttelse af personlige oplysninger
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: 24721325aefd4a8c0dbeb7864ce6da637c4df932694d4b6fff80cab5bb5b4319
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114166"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge konfigurere indstillinger for beskyttelse af personlige oplysninger

Hvis en Microsoft Edge ikke-internetbaserede platforme, Windows sendes diagnostiske data og webstedsoplysninger som standard ikke til Microsoft. Men hvis Microsoft Edge installeret på Windows 10, sendes diagnostiske data og webstedsoplysninger i henhold til Windows [indstillinger for diagnostiske data.](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)

Hvis du vil konfigurere Microsoft Edge hvordan dataindsamling for organisationen skal håndteres, skal du bruge følgende gruppepolitikker:
- [MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): Denne politik gør det muligt at rapportere om brug og data, der er relateret til nedbrud.
- [SendSiteInfoToImproveServices:](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices)Denne politik sender webstedsoplysninger, der bruges til at forbedre Microsoft-tjenester.

Du kan få mere at vide under [Konfigurer politikindstillinger.](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings)