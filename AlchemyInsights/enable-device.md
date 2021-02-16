---
title: Aktivér enhed
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8278"
ms.openlocfilehash: 9e4b03dcba7a2c98a5d63213ee49f9ba8f91d670
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256758"
---
# <a name="enable-device"></a>Aktivér enhed

**Sådan aktiveres enheden ved hjælp af kommandoen Powershell**

Kør følgende kommandoer:

- Sådan henter du enhedsobjekt: `Get-MsolDevice -Name <Name>`
- Sådan aktiveres enheden: `Enable-MsolDevice -DeviceId <DeviceId>`

Du kan finde flere oplysninger om konfiguration af hybrid joinforbindelse på administrerede domæner under [Konfigurer hybrid joinforbindelse.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains)
