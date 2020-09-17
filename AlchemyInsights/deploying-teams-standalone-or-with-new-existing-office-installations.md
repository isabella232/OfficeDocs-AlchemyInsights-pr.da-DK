---
title: Installation af teams som enkeltstående eller med nye eller eksisterende Office-installationer
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
ms.openlocfilehash: c3ca4365abc41509ccf602c5b9046655706840fc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806753"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Installation af teams som enkeltstående eller med nye eller eksisterende Office-installationer

Microsoft teams er nu inkluderet som en del af ***nye installationer*** af Microsoft 365-apps til Enterprise, Microsoft 365 apps til Business og Office til Mac. Hvis du vil have mere at vide, skal du se [Hvornår kommer Microsoft teams i gang med at inkludere nye installationer af Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Desuden vil teams, der starter med version 1906 i aktuel kanal, blive ***føjet til eksisterende installationer*** af Microsoft 365-apps til Enterprise (og Microsoft 365-apps til virksomheder) på enheder, der kører Windows, når du opdaterer din eksisterende installation til den nyeste version. Hvis du vil have mere at vide, skal du se [Hvad med eksisterende installationer af Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Hvis du ikke vil vente på denne plan for distribution, kan du installere teams som enkeltstående for dine brugere ved at [følge disse instruktioner](https://docs.microsoft.com/MicrosoftTeams/msi-deployment),   eller du kan få dine brugere til selv at installere teams fra  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Hvis din organisation ikke er klar til at installere teams, har vi de trin, du kan tage for at ***udelukke teams*** fra [nye](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) eller [eksisterende](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) installationer af Office. Hvis du vil have teams til at blive installeret, men du ikke ønsker, at teams skal starte automatisk for brugeren, når det er installeret, skal du se [forhindre Microsoft team i at starte automatisk efter installationen](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Hvis du vil ***fjerne teams*** fra en enhed, der kører Windows, skal du se [fjerne Microsoft teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Hvis du vil rydde op i Microsoft teams fra flere destinationscomputere eller-brugere, skal du se [Oprydning af Microsoft teams](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Hvis du bruger delte computere, Fjernskrivebord-tjenester (RDS) eller virtuel skrivebords infrastruktur (VDI), skal du se [Shared computer-og VDI-miljøer med Microsoft teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Hvis du bruger Office til Mac, skal du se [Microsoft teams-installationer på en Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Når teams er installeret, [opdateres det automatisk](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) cirka hver anden uge med nye funktioner og kvalitetsopdateringer. 