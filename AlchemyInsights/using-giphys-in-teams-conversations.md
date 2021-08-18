---
title: Brug af Giphys Teams samtaler
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
ms.openlocfilehash: 296c2f80d35f1c93ab3c60e0be65fd96c953ca81
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323514"
---
# <a name="using-giphys-in-teams-conversations"></a>Brug af Giphys Teams samtaler

Giphys-adgang Teams chat er aktiveret som standard. Som administrator kan du styre, om Giphys [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) er tilgængelig for brugere ved at angive en beskedpolitik og sikre, at Brug **Giphys i samtaler** er **til**.

Hvis GIF-filer ikke fungerer som forventet i Teams, skal du kontrollere følgende:

Beskedpolitikken [skal](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) tillade Giphys. Sådan kontrollerer du ved hjælp af PowerShell-cmdlet'er:

- Kontrollér, at du [kan Teams med PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)
- Kør PowerShell-kommandoen [Get-CsTeamsMessagingPolicy -Identity Global,](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) og bekræft, at **AllowGiphy** er indstillet til **SAND.**
- Hvis **AllowGiphy er** indstillet til **FALSK,** skal du køre følgende PowerShell-kommando [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Valgfrie forbundne](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) oplevelser skal være aktiveret for at tillade adgang til Giphy-URL-adressen.

**Bemærk!** Hvis du har flere Teams Messaging-politikker, der er konfigureret for din lejer, kan du bestemme identiteten af den politik, der er tildelt den påvirkede bruger, ved hjælp af [PowerShell-kommandoen Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Vælg TeamsMessagingPolicy.
