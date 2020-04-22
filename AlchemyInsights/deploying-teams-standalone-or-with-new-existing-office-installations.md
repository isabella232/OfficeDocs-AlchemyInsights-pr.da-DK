---
title: Implementering af teams som enkeltstående eller med nye eller eksisterende Office-installationer
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 4b843407f05db207f3b676c03c7088d3d0ba062e
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704627"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Implementering af teams som enkeltstående eller med nye eller eksisterende Office-installationer

Microsoft Teams er nu inkluderet som en del af ***nye installationer*** af Microsoft 365 Apps til virksomheder, Microsoft 365 Apps til virksomheder og Office til Mac. Du kan finde flere oplysninger under [Hvornår begynder Microsoft Teams at indgå med nye installationer af Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)

Fra og med Version 1906 i Månedlig kanal føjes Teams desuden ***til eksisterende installationer*** af Microsoft 365 Apps til virksomheder (og Microsoft 365 Apps til virksomheder) på enheder, der kører Windows, når du opdaterer din eksisterende installation til den nyeste version. Du kan finde flere oplysninger under [Hvad med eksisterende installationer af Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)

> [!NOTE]
> Hvis du ikke vil vente på denne udrulningsplan, kan du installere Teams som enkeltstående for dine brugere ved [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads)at følge disse [instruktioner,](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) eller du kan få brugerne til at installere Teams for sig selv fra .

Hvis din organisation ikke er klar til at installere Teams, har vi de trin, du kan gøre for at ***ekskludere teams*** fra [nye](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) eller [eksisterende](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) installationer af Office. Hvis teams skal installeres, men ikke ønsker, at Teams skal starte automatisk for brugeren, når den er installeret, skal du se [Forhindre Microsoft Teams i at starte automatisk efter installationen](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Hvis du vil ***fjerne Teams*** fra en enhed, der kører Windows, skal du se Fjerne [Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Hvis du vil rydde op i Microsoft Teams fra flere destinationsmaskiner eller -brugere, skal du se [Oprydning i microsoft Teams-installation](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Hvis du bruger delte computere, RDS (Remote Desktop Services) eller VDI (Virtual Desktop Infrastructure), skal du se [Delte computer- og VDI-miljøer med Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Hvis du bruger Office til Mac, skal du se [Microsoft Teams-installationer på en Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Når Teams er installeret, [opdateres](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) den automatisk ca. hver anden uge med nye funktioner og kvalitetsopdateringer. 