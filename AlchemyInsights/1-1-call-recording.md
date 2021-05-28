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
ms.openlocfilehash: 18c68fee514681b2a81c3cfa022c29ce83834f22
ms.sourcegitcommit: 610a5d950cdf488870601762ef52d881e3e22a48
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696916"
---
# <a name="11-call-recording"></a>1:1 opkaldsoptagelse

Hvis knappen **Start optagelse** er nedtonet i et 1:1-opkald, skal du ændre politikindstillingerne for den påvirkede bruger.   

Fra og med den 31. maj 2021 begynder vi at håndhæve en ny Teams-opkaldspolitik *AllowCloudRecordingForCalls*. Før denne ændring styres 1:1-opkaldsoptagelse af *politikken AllowCloudRecording* Teams Meeting Policy. Denne ændring er dokumenteret i indlægget i Meddelelsescenter: [(Opdateret) 1:1 Introduktion til](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)optagelsespolitik for opkald.  

*AllowCloudRecordingForCalls*   opkaldspolitik er indstillet til **$False** som standard. Hvis du foretrækker at blokere alle brugere fra at optage 1:1-opkald, behøver du ikke at foretage dig noget.  

For at aktivere opkaldsoptagelse for alle brugere i 1:1-opkald skal Teams PowerShell til at køre følgende cmdlet: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Alternativt kan du oprette en ny politik og indstille **AllowCloudRecordingForCalls** **til at $true** og tildele denne politik til dine brugere. 

Du kan få mere at vide [under 1:1 Politikkontrolelementer for opkaldsoptagelse er (næsten!) Her](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
