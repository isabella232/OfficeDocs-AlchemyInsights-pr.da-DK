---
title: 1:1 opkaldsoptagelse
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733843"
---
# <a name="11-call-recording"></a>1:1 opkaldsoptagelse

Administratorer skal handle nu for at fortsætte med at tillade brugere at optage 1:1-opkald.
 
Fra og med 12. april 2021 begynder vi at håndhæve en ny indstilling for Teams-opkaldspolitik *AllowCloudRecordingForCalls.* 

I øjeblikket styres 1:1-opkaldsoptagelsesfunktionerne af *indstillingen AllowCloudRecording* i Teams-mødepolitikker. Hvis dine brugere har tilladelse til at optage Teams-møder, kan de også optage 1:1-opkald.

Hvis du foretrækker at blokere alle brugere fra at optage 1:1-opkald, behøver du ikke at foretage dig noget. *Indstillingen AllowCloudRecordingForCalls-opkaldspolitik* ændres $False som standard.

Denne ændring er dokumenteret i følgende indlæg i Meddelelsescenter: [(Opdateret) 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) Introduktion til politik for optagelse af opkald For at konfigurere politikindstillingen for Teams-opkaldspolitik skal du bruge [Teams PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-install)

**Sådan aktiverer du opkaldsoptagelse i 1:1-opkald:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True

**Sådan deaktiverer du opkaldsoptagelse i 1:1-opkald:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False

