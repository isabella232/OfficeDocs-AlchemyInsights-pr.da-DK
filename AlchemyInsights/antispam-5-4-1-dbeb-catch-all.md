---
title: AntiSpam 5.4.1 DBEB catch-all
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
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707905"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Løs leveringsproblemer for fejlkode 550 5.4.1 Relay Access Denied

Dette problem opstÃ¥r, [nÃ¥r du kontrollerer, om en mailadresse er gyldig for at forhindre afvisninger,](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) nÃ¥r du kommer ind i Microsoft-netværket. Prøv følgende:

1. Find ud af, om problemet er specifikt for et helt domæne eller en enkelt mailadresse:
    - Hele domænet: Nogle gange skal domænet synkroniseres. prøv [at indstille domænet til Intern og derefter tilbage til Autoritativ](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Enkelt e-mail-adresse: Nogle gange skal adressen synkroniseres. ændre smtp proxy-adresse og derefter ændre det tilbage kan hjælpe.
2. Find ud af, om problemet er specifikt for en gruppe eller en offentlig mappe. For nogle objekttyper skal objekterne muligvis oprettes manuelt i Azure Active Directory.

Hvis du har brug for yderligere hjælp, skal du åbne en supportbillet og angive problemets omfang (herunder den type objekt, du sender til), så vi kan hjælpe dig bedre.