---
title: Brug af Giphys i team samtaler
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
- "9003825"
- "6850"
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982461"
---
# <a name="using-giphys-in-teams-conversations"></a>Brug af Giphys i team samtaler

Giphys adgang i team chat er aktiveret som standard. Som administrator kan du kontrollere, om Giphys er tilgængelige for brugerne, ved at [angive en meddelelses politik](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) og sikre, at **brugen af Giphys i samtaler** er **slået til**.

Hvis GIF-filer ikke fungerer som forventet i team samtaler, skal du kontrollere:

[Meddelelses politikken](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) skal tillade Giphys. Sådan bekræfter du ved hjælp af PowerShell-cmdletter:

- Kontrollér, at du kan [administrere teams med PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Kør PowerShell-kommandoen [Get-CsTeamsMessagingPolicy-Identity global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) , og kontrollér, at **AllowGiphy** er angivet til **sand**.
- Hvis **AllowGiphy** er indstillet til **falsk** , skal du køre følgende PowerShell [-kommando set-CsTeamsMessagingPolicy-Identity global-AllowGiphy $true](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Valgfrie forbundne oplevelser](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) skal være aktiveret, for at du kan få adgang til Giphy-URL-adressen.

> [!NOTE]
> Hvis du har flere teams-meddelelses politikker konfigureret for din lejer, kan du bestemme identiteten af den politik, der er tildelt den påvirkede bruger, med PowerShell [-kommandoen Get-CsOnlineUser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Vælg TeamsMessagingPolicy.
