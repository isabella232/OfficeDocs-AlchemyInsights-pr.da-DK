---
title: Microsoft Edge Konfigurer indstillinger for beskyttelse af personlige oplysninger
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
ms.openlocfilehash: dcd1d91dcde1f585caf0e1e3af30946513a0f26c
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677249"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge Konfigurer indstillinger for beskyttelse af personlige oplysninger

Hvis Microsoft Edge er installeret på ikke-Windows-platforme, sendes der som standard ikke diagnostiske data og websteds oplysninger til Microsoft. Men hvis Microsoft Edge installeres på Windows 10, sendes diagnostiske data og websteds oplysninger i henhold til brugernes [Indstillinger for Windows-diagnosticeringsdata](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).

Hvis du vil konfigurere, hvordan Microsoft Edge håndterer dataindsamling for din organisation, skal du bruge følgende gruppepolitikker:
- [MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): denne politik aktiverer rapportering af anvendelses-og crash-relaterede data.
- [SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): denne politik sender oplysninger om webstedet, der bruges til at forbedre Microsoft-tjenester.

Hvis du vil have mere at vide, skal du se [konfigurere politikindstillinger](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).