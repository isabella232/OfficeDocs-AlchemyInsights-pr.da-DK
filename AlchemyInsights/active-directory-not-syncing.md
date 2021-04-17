---
title: Active Directory synkroniseres ikke
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
- "9001688"
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822845"
---
# <a name="active-directory-not-syncing"></a>Active Directory synkroniseres ikke

Hvis du modtager synkroniseringsfejl, f.eks. "ingen seneste synkronisering", eller bemærker status for katalogsynkronisering i Office-administrationsportalen siger "Senest synkroniseret for mere end 3 dage siden", kan det være, at AADConnect har forkerte indstillinger eller utilstrækkelige tilladelser til at udføre en synkronisering.  

Hvis du geninstallerer AADConnect ved hjælp af hurtig konfiguration, kan problemet muligvis løses hurtigt:

1. [Download den nyeste version af AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Følg vejledningen for hurtig installation.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)

Du kan finde flere oplysninger om AADConnect-tjenestekonti [i Azure AD Connect: Konti og tilladelser.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)
