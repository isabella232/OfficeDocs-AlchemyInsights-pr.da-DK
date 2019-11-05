---
title: AntiSpam 5.4.1 DBEB catch-alle
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: 4a56cfe74d8940e53a316d3bcc3809e8666c2e37
ms.sourcegitcommit: a8945ab0008f138b2992175b0640e78a505d29e1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 11/04/2019
ms.locfileid: "37964107"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Løs problemer med levering af fejlkode 550 5.4.1 relæ adgang nægtet

Dette problem opstår, når du [tjekker, om en e-mail-adresse er gyldig for at forhindre tilbageslag](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) , når du indtaster Office 365-netværket. Prøv følgende:

1. Bestem, om problemet er specifikt for et helt domæne eller en enkelt e-mail-adresse:
    - Hele domænet: nogle gange skal domænet synkroniseres. Prøv at [indstille domænet til internt og derefter tilbage til autoritativ](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
     - Enkelt e-mail-adresse: nogle gange skal adressen synkroniseres. Det kan hjælpe at ændre SMTP-proxyadressen og derefter ændre den igen.
2. Find ud af, om problemet er specifikt for en gruppe eller en offentlig mappe. For nogle objekttyper skal objekterne muligvis oprettes manuelt i Azure Active Directory.

Hvis du har brug for yderligere hjælp, skal du åbne en support billet og angive omfanget af problemet (Inkluder den type objekt, du sender til), så vi kan hjælpe dig bedre.