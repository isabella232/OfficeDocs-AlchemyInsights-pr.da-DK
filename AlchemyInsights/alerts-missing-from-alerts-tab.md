---
title: Beskeder mangler under fanen Beskeder
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12732"
ms.openlocfilehash: 9fbd9a32e40d858f0ba49931c723a824478aaa12
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/16/2021
ms.locfileid: "58454534"
---
# <a name="alerts-missing-from-alerts-tab"></a>Beskeder mangler under fanen Beskeder

Fanen **Vigtige beskeder** fungerer baseret på konfiguration og aktiverede politikker fra portalen til appstyring i din lejer. Out of the box-politikker i appstyring skal også aktiveres for at lade signaler flyde til **fanen Vigtige** beskeder. 

Bekræft, at beskeden er blevet oprettet:

1. Gå til Politikker for [appstyring,](https://compliance.microsoft.com/m365appprotection?viewid=policies) og bekræft, at du har oprettet mindst én aktiv eller overvågningspolitik.

1. Vælg politikken, og seleect **Rediger i** pop op-ruden. 

1. Kontrollér politikkonfigurationen for at bekræfte, at der skulle være oprettet en besked baseret på en politikhændelse, der blev startet for mere end 24 timer siden.

Du kan finde flere oplysninger om beskeder om appstyring i Introduktion til registrering og afhjælpning af [trusler i apps.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-detect-remediate-get-started)