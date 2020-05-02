---
title: Privat kanal
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005432"
---
# <a name="private-channels-in-microsoft-teams"></a>Private kanaler i Microsoft Teams

Private kanaler er en ny funktion i Microsoft Teams. Bemærk, at private kanaler ikke kan konverteres fra standardkanaler eller omvendt.

Du kan finde flere oplysninger [private channel creation and membership](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) om private kanaler, [private channel SharePoint sites](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites) [f.eks.](https://docs.microsoft.com/MicrosoftTeams/private-channels) 

**Bemærk:** Da konfiguration til opbevaring af private kanalmeddelelser endnu ikke understøttes, vil lejere med opbevaringspolitikker aktiveret ikke have private kanaler aktiveret som standard. Private kanaler kan aktiveres i Teams Administration. Bemærk også, at selvom opbevaring af private kanalbeskeder ikke understøttes, understøttes opbevaring af filer, der deles i private kanaler.

**Har du brug for en ny teamejer?**

Hvis din private kanalejer forlader den, kan du tilføje en ny teamejer via Teams Powershell.


- Gå [her](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) for at installere Teams Powershell.

Her er den cmdlet, du skal bruge:

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

Yderligere oplysninger om Teams Powershell finder du i [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).
