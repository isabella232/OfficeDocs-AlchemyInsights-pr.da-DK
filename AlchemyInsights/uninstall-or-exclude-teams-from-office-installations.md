---
title: Fjern eller Udelad teams fra Office-installationer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2662"
- "9000660"
ms.openlocfilehash: 22d69db749671afdfe7a809d1bc598e2ad1891d8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658215"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a>Fjern eller Udelad teams fra nye eller eksisterende Office-installationer

Microsoft teams er inkluderet som en del af Microsoft 365-apps til Enterprise, Microsoft 365-apps til Business og Office til Mac.

- Brug [Office-udrulnings værktøjet](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) til at udelukke teams fra nye installationer af Office.
- Hvis du vil *fjerne* teams fra en enhed, der kører Windows, skal du se [fjerne Microsoft teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Hvis du vil rydde op i Microsoft teams fra flere destinationscomputere eller-brugere, skal du se [Oprydning af Microsoft teams-udrulning](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).
- Brug indstillingen [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) for at forhindre Microsoft team i at blive installeret automatisk sammen med Office.
- Brug indstillingen [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) , *før teams er installeret*, for at forhindre Microsoft team i at starte automatisk efter installationen.

Hvis du bruger Office til Mac, skal du se [Microsoft teams-installationer på en Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).