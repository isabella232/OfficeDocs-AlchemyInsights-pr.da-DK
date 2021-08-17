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
ms.openlocfilehash: c17408442cec6c0877b7d66bc8a7fd3062eb0e47
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314378"
---
# <a name="11-call-recording"></a>1:1 opkaldsoptagelse

Hvis knappen **Start optagelse** er nedtonet i et 1:1-opkald, skal du ændre politikindstillingerne for den påvirkede bruger. Du kan kontrollere politikindstillingen ved at køre Diagnosticering for den på påvirkede bruger ved at skrive **Diag: Teams 1:1 opkaldsoptagelse** ovenfor.     

Fra og med den 31. maj 2021 begynder vi at gennemtvinge en ny Teams-opkaldspolitik *TilladCloudRecordingForCalls*. Før denne ændring styres 1:1-opkaldsoptagelse af *Politikken AllowCloudRecording* Teams Meeting Policy. Denne ændring er dokumenteret i indlægget i Meddelelsescenter: [(Opdateret) 1:1 Introduktion til](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)optagelsespolitik for opkald.  

*AllowCloudRecordingForCalls*   opkaldspolitik er indstillet til **$False** som standard. Hvis du foretrækker at blokere alle brugere fra at optage 1:1-opkald, behøver du ikke at foretage dig noget.  

For at aktivere opkaldsoptagelse for alle brugere i 1:1-opkald [skal Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install) til at køre følgende cmdlet: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Alternativt kan du oprette en ny politik og indstille **AllowCloudRecordingForCalls** **til at $true** og tildele denne politik til dine brugere. 

Du kan få mere at vide [under 1:1 Politikkontrolelementer for opkaldsoptagelse er (næsten!) Her](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
