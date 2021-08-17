---
title: Sådan aktiveres Hosted Voicemail
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 4d70e92a7c1bf8f3cc62d4a310aa140ee2dfdef4c798ae17faa961736d9db500
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055548"
---
# <a name="how-to-enable-hosted-voicemail"></a>Sådan aktiveres Hosted Voicemail

For at aktivere Voicemail skal **HostedVoicemail** være indstillet til $true.

Egenskaben **HostedVoicemail** for brugeren ved hjælp af Remote PowerShell (RPS).

Du kan finde flere oplysninger om at oprette forbindelse til RPS [Microsoft Teams Oversigt over PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for at få flere oplysninger om at oprette forbindelse til RPS.

1. Den Teams administrator skal være logget på Remote PowerShell for at Teams.
1. Fra PowerShell-prompten kan Teams-administratoren køre **set-csuser user@contoso.com -HostedVoiceMail $true** hvor sip uri'en er af den pågældende bruger.

> [!NOTE]
> Det kan tage op til 24 timer at replikere ændringer i politikker.