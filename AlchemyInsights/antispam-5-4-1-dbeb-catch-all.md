---
title: AntiSpam 5.4.1 DBEB catch-all
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
- "9001209"
- "3167"
ms.openlocfilehash: e0e9b4fec0615943227f40043aeed842e8ee556c5916a59f65e79ce121ec9547
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932271"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Løs leveringsproblemer for fejlkode 550 5.4.1 Relay Access Denied

Dette problem opstår, når [du kontrollerer, om en mailadresse er](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) gyldig, for at forhindre tilbageførsel ved indtastning af Microsoft-netværket. Prøv følgende:

1. Afgør, om problemet er specifikt for et helt domæne eller en enkelt mailadresse:
    - Hele domænet: Nogle gange skal domænet synkroniseres; prøv [at indstille domænet til Intern og derefter tilbage til Autoritativ](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Enkelt mailadresse: Nogle gange skal adressen synkroniseres; det kan hjælpe at ændre smtp-proxyadressen og derefter ændre den tilbage.
2. Afgør, om problemet er specifikt for en gruppe eller offentlig mappe. For nogle objekttyper skal objekterne muligvis oprettes manuelt i Azure Active Directory.

Hvis du har brug for yderligere hjælp, skal du åbne en supportbillet og angive problemets omfang (herunder typen af objekt, du sender til), så vi kan hjælpe dig bedre.