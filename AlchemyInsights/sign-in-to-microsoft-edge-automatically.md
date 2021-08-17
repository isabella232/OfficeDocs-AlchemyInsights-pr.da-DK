---
title: Log på Microsoft Edge
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
ms.openlocfilehash: 4e069a1c75caabf3bef7387140edd5650cf966856b888b5c6b5618a603986d6d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050688"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Log på Microsoft Edge

Microsoft Edge bruger OS-standardkontoen til automatisk at logge en bruger på, afhængigt af hvordan brugerens enhed er konfigureret. 

Scenarierne for hver type enhedskonfiguration og den afhængige brugers logonproces er beskrevet nedenfor:

- **Enheden er hybrid/AAD-J:** Denne indstilling er tilgængelig på Windows 10, niveau Windows og tilsvarende serverversioner. Brugere logges automatisk på med deres Azure Active Directory (AD)-konti.
- **Enheden er domæneforbundne:** Denne indstilling er tilgængelig på Windows 10, versioner på Windows niveau og tilsvarende serverversioner. Som standard er brugere med domænekonti ikke logget på automatisk. Hvis du vil aktivere automatisk logon for dem, skal du bruge **politikken ConfigureOnPremisesAccountAutoSignIn.** Hvis du vil aktivere automatisk logon for brugere med Azure AD-konti, bør du overveje at deltage hybridt i deres enheder.
- **Operativsystemets** standardkonto er en Microsoft-konto: Denne indstilling er tilgængelig på Windows 10 RS3 (version 1709, build 10.0.16299) og nyere versioner. Det er usandsynligt, at scenariet forekommer på virksomhedsenheder. Men hvis OS-standardkontoen er en Microsoft-konto, Microsoft Edge logges der automatisk på brugeren med Microsoft-kontoen.
 
 
