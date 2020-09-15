---
title: Spam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717355"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Løs leverings problemer for fejlkode 550 5.4.1 Relay-adgang nægtet

Dette problem opstår, når du [kontrollerer, om en mailadresse er gyldig for at forhindre bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) , når du angiver Microsoft-netværket. Prøv følgende:

1. Find ud af, om problemet er specifikt for et helt domæne eller en enkelt mailadresse:
    - Hele domænet: nogle gange skal domænet synkroniseres. Prøv at [indstille domænet til internt og derefter tilbage til autoritativ](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Enkelt mailadresse: det er nogle gange, at adressen skal synkroniseres. Hvis du ændrer SMTP-proxyadressen og derefter ændrer den tilbage, kan det hjælpe.
2. Find ud af, om problemet er specifikt for en gruppe eller en offentlig mappe. For nogle objekttyper skal objekterne muligvis oprettes manuelt i Azure Active Directory.

Hvis du har brug for yderligere hjælp, skal du åbne en supportanmodning og angive omfanget af problemet (herunder den type objekt, du sender til), så vi kan hjælpe dig bedre.