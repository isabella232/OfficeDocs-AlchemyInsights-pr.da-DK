---
title: Fjern eller udelad Teams fra Office-installationer
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2662"
- "9000660"
ms.openlocfilehash: 2d96d54cb479f5f52cc707d4307cf9cf1e891a01
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827786"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a>Fjern eller udelad Teams fra nye eller eksisterende Office-installationer

Microsoft Teams er inkluderet som en del af Microsoft 365 Apps til store virksomheder, Microsoft 365 Apps til virksomheder og Office til Mac.

- Brug [Office Udrulningsværktøj](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) til at udelukke Teams fra nye installationer af Office.
- Hvis du *vil* fjerne Teams fra en enhed, der kører Windows, skal [du se Fjern Microsoft Teams.](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81) Hvis du vil rydde op i Microsoft Teams fra flere destinationscomputere eller -brugere, skal du [se Oprydning af installation i Microsoft Teams](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).
- Brug indstillingen [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) til at forhindre Microsoft Teams i at installere automatisk med Office.
- Brug indstillingen [PreventFirstLaunchAfterInstall,](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) før *Teams* er installeret, for at forhindre, at Microsoft Teams starter automatisk efter installationen.

Hvis du bruger Office til Mac, skal du se [Microsoft Teams-installationer på en Mac.](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)