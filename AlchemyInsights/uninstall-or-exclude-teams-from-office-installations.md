---
title: Fjerne eller ekskludere teams fra Office-installationer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2662"
- "9000660"
ms.openlocfilehash: b6613733e743e08a9b18b1ada70fde164b0d5dc3
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010285"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a>Fjerne eller ekskludere teams fra nye eller eksisterende Office-installationer

Microsoft Teams er inkluderet som en del af Microsoft 365 Apps til virksomheder, Microsoft 365 Apps til virksomheder og Office til Mac.

- Brug [Office-installationsværktøjet](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) til at udelukke teams fra nye installationer af Office.
- Hvis du vil *fjerne* Teams fra en enhed, der kører Windows, skal du se [Fjerne Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Hvis du vil rydde op i Microsoft Teams fra flere destinationsmaskiner eller brugere, skal du se [Oprydning i microsoft Teams-installation](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).
- Brug indstillingen [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) til at forhindre Microsoft Teams i at installere automatisk med Office.
- Brug indstillingen [PreventFirstLaunchAfterInstall,](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) *før Teams installeres*, for at forhindre Microsoft Teams i at starte automatisk efter installationen.

Hvis du bruger Office til Mac, skal du se [Microsoft Teams-installationer på en Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).