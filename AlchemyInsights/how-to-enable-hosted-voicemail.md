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
ms.openlocfilehash: 4042e042554f78febff2073fde6f14db72a6d4e0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318642"
---
# <a name="how-to-enable-hosted-voicemail"></a>Sådan aktiveres Hosted Voicemail

For at aktivere Voicemail skal **HostedVoicemail** være indstillet til $true.

Egenskaben **HostedVoicemail** for brugeren ved hjælp af Remote PowerShell (RPS).

Du kan finde flere oplysninger om at oprette forbindelse til RPS Microsoft Teams Oversigt over [PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for at få flere oplysninger om at oprette forbindelse til RPS.

1. Den Teams administrator skal være logget på Remote PowerShell for Teams.
1. Fra PowerShell-prompten kan Teams-administratoren køre **set-csuser user@contoso.com -HostedVoiceMail $true** hvor sip uri'en er af den pågældende bruger.

**Bemærk!** Det kan tage op til 24 timer at replikere ændringer i politikker.