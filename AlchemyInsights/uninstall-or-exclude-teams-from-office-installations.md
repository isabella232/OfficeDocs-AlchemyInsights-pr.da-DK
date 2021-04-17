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
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="8eab2-102">Fjern eller udelad Teams fra nye eller eksisterende Office-installationer</span><span class="sxs-lookup"><span data-stu-id="8eab2-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="8eab2-103">Microsoft Teams er inkluderet som en del af Microsoft 365 Apps til store virksomheder, Microsoft 365 Apps til virksomheder og Office til Mac.</span><span class="sxs-lookup"><span data-stu-id="8eab2-103">Microsoft Teams is included as part of Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business, and Office for Mac.</span></span>

- <span data-ttu-id="8eab2-104">Brug [Office Udrulningsværktøj](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) til at udelukke Teams fra nye installationer af Office.</span><span class="sxs-lookup"><span data-stu-id="8eab2-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="8eab2-105">Hvis du *vil* fjerne Teams fra en enhed, der kører Windows, skal [du se Fjern Microsoft Teams.](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)</span><span class="sxs-lookup"><span data-stu-id="8eab2-105">To *uninstall* Teams from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="8eab2-106">Hvis du vil rydde op i Microsoft Teams fra flere destinationscomputere eller -brugere, skal du [se Oprydning af installation i Microsoft Teams](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span><span class="sxs-lookup"><span data-stu-id="8eab2-106">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="8eab2-107">Brug indstillingen [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) til at forhindre Microsoft Teams i at installere automatisk med Office.</span><span class="sxs-lookup"><span data-stu-id="8eab2-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="8eab2-108">Brug indstillingen [PreventFirstLaunchAfterInstall,](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) før *Teams* er installeret, for at forhindre, at Microsoft Teams starter automatisk efter installationen.</span><span class="sxs-lookup"><span data-stu-id="8eab2-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="8eab2-109">Hvis du bruger Office til Mac, skal du se [Microsoft Teams-installationer på en Mac.](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)</span><span class="sxs-lookup"><span data-stu-id="8eab2-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>