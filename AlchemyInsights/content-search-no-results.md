---
title: Indhold søgeresultater ikke
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800266"
---
# <a name="no-results-from-content-searchexports"></a>Ingen resultater fra indhold Søg/eksport

Problemer med indhold Søg/eksport ikke returnere data, kan skyldes, at visse overholdelse sikkerhedsfilter, der var opsætning ved en bestemt Admin og kommunikerer ikke til alle administratorer.

Du kan løse dette ved at kontrollere for at se, om der er nogen overensstemmelse sikkerhedsfiltre, som kan forårsage dette:
1. Oprette forbindelse til sikkerhed og Overholdelsescenter Powershell
2. Kør følgende cmdlet'er:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-organisation $org