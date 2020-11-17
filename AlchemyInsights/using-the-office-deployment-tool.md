---
title: Brug af Office-udrulnings værktøjet
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085826"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="87f56-102">Brug af Office udrulnings værktøj (ODT)</span><span class="sxs-lookup"><span data-stu-id="87f56-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="87f56-103">Du bruger Office udrulnings værktøj (ODT) til at installere Office 365-versioner af Office.</span><span class="sxs-lookup"><span data-stu-id="87f56-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="87f56-104">Office udrulnings værktøj (setupodt.exe) køres fra kommandolinjen og bruger en XML-konfigurationsfil til at bestemme, hvilke indstillinger der skal anvendes, når du installerer Office.</span><span class="sxs-lookup"><span data-stu-id="87f56-104">The Office Deployment Tool (setupodt.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="87f56-105">Hent den nyeste version af Office-udrulnings værktøjet fra [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="87f56-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="87f56-106">Brug [Office-tilpasnings værktøjet (okt)](https://config.office.com) til at vælge dine installations præferencer og oprette XML-konfigurationsfilen.</span><span class="sxs-lookup"><span data-stu-id="87f56-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="87f56-107">Eksportér konfigurationsfilen, og sæt den lokalt på den samme mappe, hvor setupodt.exe er placeret.</span><span class="sxs-lookup"><span data-stu-id="87f56-107">Export the configuration file and place it locally on the same folder where the setupodt.exe resides.</span></span>

    <span data-ttu-id="87f56-108">**Bemærk:** Office-installationsproblemer opstår ofte på grund af forkert konfigurerede eller malformatted-konfigurationsfiler.</span><span class="sxs-lookup"><span data-stu-id="87f56-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="87f56-109">For at undgå sådanne problemer anbefaler vi, at du bruger Office-tilpasnings værktøjet til at oprette konfigurationsfilen.</span><span class="sxs-lookup"><span data-stu-id="87f56-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="87f56-110">Du kan også importere eksisterende konfigurationsfiler til Office-tilpasnings værktøjet.</span><span class="sxs-lookup"><span data-stu-id="87f56-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="87f56-111">Fra en kommandoprompt med administratorrettigheder skal du skifte til den placering, hvor setupodt.exe er placeret, og køre Office-udrulnings værktøjet i overførselstilstand og angive den konfigurationsfil, du lige har gemt.</span><span class="sxs-lookup"><span data-stu-id="87f56-111">From an elevated command prompt, switch to the location where setupodt.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="87f56-112">I dette eksempel hedder konfigurationsfilen Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="87f56-112">In this example, the configuration file is named Configuration.xml:</span></span>

```setupodt.exe /download Configuration.xml```

<span data-ttu-id="87f56-113">4. Kør Office-udrulnings værktøjet i konfigurationstilstand, og Angiv konfigurationsfilen.</span><span class="sxs-lookup"><span data-stu-id="87f56-113">4.Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>

```setupodt.exe /configure Configuration.xml```

<span data-ttu-id="87f56-114">**Bemærk:** Du skal køre dette trin fra den klientcomputer, hvor du vil installere Office, og du skal have lokale administratorrettigheder på den computer.</span><span class="sxs-lookup"><span data-stu-id="87f56-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="87f56-115">Du kan få mere at vide om, hvordan du bruger Office-udrulnings værktøjet til dine Microsoft 365-apps til virksomheds installationsscenarier, under [Oversigt over Office-udrulnings værktøjet](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="87f56-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span></span> <span data-ttu-id="87f56-116">Du kan finde flere oplysninger om, hvordan du bruger Office-tilpasnings værktøjet, under [Oversigt over Office-tilpasnings værktøjet](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="87f56-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
