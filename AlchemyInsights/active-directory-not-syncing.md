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
ms.openlocfilehash: d4615d335b9aeef69148cd93ff9f44bec6d7d876
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314198"
---
# <a name="active-directory-not-syncing"></a>Active Directory synkroniseres ikke

Hvis du modtager synkroniseringsfejl, f.eks. "ingen seneste synkronisering", eller bemærker status for katalogsynkronisering i Office-administrationsportalen siger "Senest synkroniseret for mere end 3 dage siden", kan det være, at AADConnect har forkerte indstillinger eller utilstrækkelige tilladelser til at udføre en synkronisering.  

Hvis du geninstallerer AADConnect ved hjælp af hurtig konfiguration, kan problemet muligvis løses hurtigt:

1. [Download den nyeste version af AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Følg vejledningen for hurtig installation.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)

Azure AD Connect skal installeres på Windows Server 2012 eller nyere. Denne server skal være tilknyttet et domæne, og det kan være domænecontroller eller en medlemsserver. Du kan se en komplet liste over Forbind og forudsætninger for Azure AD ved at gennemgå Forudsætninger [for Azure AD Forbind.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites)

Du kan finde flere oplysninger om AADConnect-tjenestekonti [i Azure AD Forbind: Konti og tilladelser](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
