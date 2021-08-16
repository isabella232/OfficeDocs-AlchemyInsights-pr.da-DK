---
title: Installation Teams enkeltstående eller med nye eller eksisterende Office installationer
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: e8baefafc1c2f9583345779c5ae7a9d3d0e05c4b3b7e1b3a74a9a22f7ceed02a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102196"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Installation Teams enkeltstående eller med nye eller eksisterende Office installationer

Microsoft Teams nu inkluderet som ***en del*** af nye installationer af Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business og Office til Mac. Du kan finde flere oplysninger [under Hvornår Microsoft Teams med at blive inkluderet i nye Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Desuden føjes Teams fra version 1906 til eksisterende  installationer af Microsoft 365 Apps for enterprise (og Microsoft 365 Apps for business) på enheder, der kører Windows, når du opdaterer din eksisterende installation til den nyeste version. Du kan få mere at [vide under Hvad med eksisterende Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Hvis du ikke vil vente på denne udrulningsplan, kan du installere Teams [](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) som separat for brugerne ved at følge disse instruktioner, eller du kan få brugerne til selv at installere Teams fra [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Hvis din organisation ikke er klar til at installere Teams, har vi de trin, [](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) du kan tage for at ***udelukke Teams*** fra nye eller eksisterende Office. [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) Hvis du ønsker Teams skal være installeret, men ikke ønsker, at Teams starter automatisk for brugeren, når den er installeret, skal du se Forebyd, at Microsoft Teams starter automatisk [efter installationen.](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)

Hvis ***du vil Teams fra*** en enhed, der Windows, skal du se [Microsoft Teams.](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81) Hvis du vil rydde op Microsoft Teams fra flere destinationscomputere eller brugere, skal [Microsoft Teams rydde op i installationen.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)

Hvis du bruger delte computere, RDS (Remote Desktop Services) eller VDI (Virtual Desktop Infrastructure), skal du se Delte computer- og [VDI-miljøer med Microsoft Teams.](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)

Hvis du bruger en Office til Mac, skal du [Microsoft Teams på en Mac.](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)

> [!NOTE]
> Når Teams er installeret, [opdateres den automatisk ca.](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) hver anden uge med nye funktioner og kvalitetsopdateringer. 