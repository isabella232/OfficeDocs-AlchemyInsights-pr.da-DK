---
title: Sådan aktiveres hosted voicemail
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
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/09/2020
ms.locfileid: "49677336"
---
# <a name="how-to-enable-hosted-voicemail"></a>Sådan aktiveres hosted voicemail

Hvis du vil aktivere voicemail, skal du angive **HostedVoicemail** til $true.

Egenskaben **HostedVoicemail** for brugeren ved hjælp af Remote POWERSHELL (RPS).

Du kan finde flere oplysninger om at oprette forbindelse til RPS i [Microsoft teams PowerShell-oversigt](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for at få flere oplysninger om at oprette forbindelse til RPS.

1. Teams-administratoren skal være logget på Remote PowerShell til teams.
1. Fra PowerShell-Spørg teams-administratoren kan køre **set-csuser User@contoso.com-$true HostedVoiceMail** , hvor SIP-URI'en er for den pågældende bruger.

> [!NOTE]
> Ændringer af politikker kan tage op til 24 timer at replikere.