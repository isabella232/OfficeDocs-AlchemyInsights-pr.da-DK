---
title: Implementering af grupper, som enkeltstående eller med nye eller eksisterende Office-installationer
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 08/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 3318e1b17cc99e927e1011f7ca9eca8dec616d59
ms.sourcegitcommit: 4600dd4fb577bf5f5482a24616c2d9a6b81e8052
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/01/2019
ms.locfileid: "36054225"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Implementering af grupper, som enkeltstående eller med nye eller eksisterende Office-installationer

Microsoft Teams er nu inkluderet som en del af ***nye installationer*** af Office 365 ProPlus, Office 365 virksomheder og Office til Mac. Yderligere oplysninger finder du [hvor Microsoft Teams begynder der følger med nye installationer af Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)

Desuden bliver fra og med Version 1906 i månedlige kanal, Teams ***føjet til eksisterende installationer*** af Office 365 ProPlus (og Office 365-Business) på enheder, der kører Windows, når du opdaterer din eksisterende installation til den nyeste version. Yderligere oplysninger finder du [Hvad med eksisterende installationer af Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)

> [!NOTE]
> Hvis du ikke vil vente på, at denne tidsplan for implementering, kan du installere grupper som enkeltstående for brugerne ved at [følge disse instruktioner](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) eller du kan lade dine brugere med at installere grupper selv fra [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads).

Hvis din organisation ikke er klar til at implementere grupper, har vi de trin, du kan udføre for at ***udelukke Teams*** fra [Ny](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) eller [eksisterende](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) installationer af Office. Hvis du vil Teams til at blive installeret, men ikke vil Teams til at starte automatisk for brugeren, når den er installeret, finder du [Forhindre Microsoft grupper i at starte automatisk efter installationen](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Se [Afinstallere Microsoft-Team](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)til at ***fjerne grupper*** fra en enhed, der kører Windows. Til oprydning Microsoft Teams fra flere destinationscomputere eller brugere, se [installation af Microsoft-Team oprydning](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Hvis du bruger delte computere, Remote Desktop Services (RDS) eller virtuelle Desktop-infrastruktur (VDI), se [delte computer og VDI-miljøer med Microsoft-Team](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Hvis du bruger Office til Mac, kan du se [Microsoft-Team installationer på en Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Når Teams er installeret, der [automatisk opdateres](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) ca. hver anden uge med nye funktioner og opdateringer af kvalitet. 