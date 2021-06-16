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
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930969"
---
# <a name="active-directory-not-syncing"></a>Active Directory synkroniseres ikke

Hvis du modtager synkroniseringsfejl, f.eks. "ingen seneste synkronisering", eller bemærker status for katalogsynkronisering i Office-administrationsportalen, hvor der står "Senest synkroniseret for mere end 3 dage siden", kan det være, at AADConnect har forkerte indstillinger eller utilstrækkelige tilladelser til at udføre en synkronisering.  

Hvis du geninstallerer AADConnect ved hjælp af hurtig konfiguration, kan problemet muligvis løses hurtigt:

1. [Download den nyeste version af AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Følg vejledningen for hurtig installation.](/azure/active-directory/hybrid/how-to-connect-install-express)

Azure AD Connect skal installeres på Windows Server 2012 eller nyere. Denne server skal være tilknyttet et domæne, og det kan være domænecontroller eller en medlemsserver. Du kan se en komplet liste over Forbind og forudsætninger for Azure AD ved at gennemgå [Forudsætninger for Azure AD Forbind.](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)

Du kan finde flere oplysninger om AADConnect-tjenestekonti [i Azure AD Forbind: Konti og tilladelser](/azure/active-directory/hybrid/reference-connect-accounts-permissions).
