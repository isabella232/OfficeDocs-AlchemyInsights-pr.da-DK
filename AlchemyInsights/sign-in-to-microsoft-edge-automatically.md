---
title: Log automatisk på Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398723"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Log automatisk på Microsoft Edge

Microsoft Edge bruger OS-standardkontoen til automatisk at logge en bruger på i overensstemmelse med, hvordan brugerens enhed er konfigureret. 

Scenarierne for hver type enhedskonfiguration og den afhængige brugers logonproces er beskrevet nedenfor:

- **Enheden er hybrid/AAD-J: Denne** indstilling er tilgængelig i Windows 10, Windows på ned niveau og tilsvarende serverversioner. Brugere logges automatisk på med deres Azure Active Directory-konti (AD).
- **Enheden er domæne-forbundet:** Denne indstilling er tilgængelig i Windows 10, Windows på ned niveau og tilsvarende serverversioner. Som standard er brugere med domænekonti ikke logget på automatisk. hvis du vil aktivere automatisk logon for dem, skal du bruge **politikken ConfigureOnPremisesAccountAutoSignIn.** Hvis du vil aktivere automatisk logon for brugere med Azure AD-konti, kan du overveje at deltage hybridt på deres enheder.
- **Os-standardkontoen** er en Microsoft-konto: Denne indstilling er tilgængelig på Windows 10 RS3 (version 1709, build 10.0.16299) og nyere versioner. Scenariet er usandsynligt på virksomhedsenheder. Men hvis OS-standardkontoen er en Microsoft-konto, logger Microsoft Edge automatisk brugeren på med Microsoft-kontoen.
 
 
