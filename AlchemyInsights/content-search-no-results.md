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
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516773"
---
# <a name="no-results-from-content-searchexports"></a>Ingen resultater fra indhold Søg/eksport

Problemer med indhold Søg/eksport ikke returnere data, kan skyldes, at visse overholdelse sikkerhedsfilter, der var opsætning ved en bestemt Admin og kommunikerer ikke til alle administratorer.

Du kan løse dette ved at kontrollere for at se, om der er nogen overensstemmelse sikkerhedsfiltre, som kan forårsage dette:
1. Oprette forbindelse til sikkerhed og Overholdelsescenter Powershell
2. Kør følgende cmdlet'er:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-organisation $org