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
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821441"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Løs leveringsproblemer for fejlkode 550 5.4.1 Relay Access Denied

Dette problem opstår, når [du kontrollerer, om en mailadresse er](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) gyldig, for at forhindre tilbageførsel ved indtastning af Microsoft-netværket. Prøv følgende:

1. Afgør, om problemet er specifikt for et helt domæne eller en enkelt mailadresse:
    - Hele domænet: Nogle gange skal domænet synkroniseres; prøv [at indstille domænet til Intern og derefter tilbage til Autoritativ](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Enkelt mailadresse: Nogle gange skal adressen synkroniseres; det kan hjælpe at ændre smtp-proxyadressen og derefter ændre den tilbage.
2. Afgør, om problemet er specifikt for en gruppe eller offentlig mappe. For nogle objekttyper skal objekterne muligvis oprettes manuelt i Azure Active Directory.

Hvis du har brug for yderligere hjælp, skal du åbne en supportbillet og angive problemets omfang (herunder typen af objekt, du sender til), så vi kan hjælpe dig bedre.