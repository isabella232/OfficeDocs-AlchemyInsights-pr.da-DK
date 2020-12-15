---
title: Logge på Microsoft Edge automatisk
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
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677233"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Logge på Microsoft Edge automatisk

Microsoft Edge bruger OPERATIVSYSTEMETS standardkonto til automatisk at logge på en bruger, afhængigt af hvordan brugerens enhed er konfigureret. 

Scenarierne for hver type enhedskonfiguration og den afhængige brugerlogon er beskrevet nedenfor:

1. **Enheden er hybrid/Aad-J**: denne indstilling er tilgængelig på Windows 10, på et down-niveau-Windows og tilsvarende server versioner. Brugere logges automatisk på med deres Azure Active Directory-konti (AD).
2. **Enheden er domæne tilmeldt**: denne indstilling er tilgængelig på Windows 10, på et down-niveau-Windows og tilsvarende server versioner. Brugere med domænekonti er som standard ikke logget på automatisk. Hvis du vil aktivere automatisk logon for dem, skal du bruge **ConfigureOnPremisesAccountAutoSignIn** -politikken. Hvis du vil aktivere automatisk logon for brugere med Azure AD-konti, skal du overveje at oprette en hybrid forbindelse til deres enheder.
3. **Operativsystemets standardkonto er en Microsoft-konto**: denne indstilling er tilgængelig på Windows 10 RS3 (version 1709, Build 10.0.16299) og nyere versioner. Scenariet vil sandsynligvis ikke forekomme på virksomhedsenheder. Men hvis OPERATIVSYSTEMETS standardkonto er en Microsoft-konto, logger Microsoft Edge automatisk brugeren med Microsoft-kontoen.
 
 
