---
title: Ved hjælp af værktøjet Office installation
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 874bb7883bca4f062e85963a6828a771cd2dad9b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36531569"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="a62d9-102">Ved hjælp af Office Deployment Tool (ODT)</span><span class="sxs-lookup"><span data-stu-id="a62d9-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="a62d9-103">Du kan bruge Office Deployment Tool (ODT) til at installere Office 365-versioner af Office.</span><span class="sxs-lookup"><span data-stu-id="a62d9-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="a62d9-104">Værktøjet Office installation (setup.exe) køres fra kommandolinjen og bruger en XML-konfigurationsfil til at bestemme, hvilke indstillinger der skal anvendes, når du installerer Office.</span><span class="sxs-lookup"><span data-stu-id="a62d9-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="a62d9-105">Hent den nyeste version af værktøjet Office installation fra [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="a62d9-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="a62d9-106">Brug [Office Customization Tool (OCT)](https://config.office.com) til at vælge dine indstillinger for installation og oprette XML-konfigurationsfilen.</span><span class="sxs-lookup"><span data-stu-id="a62d9-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="a62d9-107">Eksportere konfigurationsfilen, og Placer den lokalt på den samme mappe, hvor setup.exe er placeret.</span><span class="sxs-lookup"><span data-stu-id="a62d9-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="a62d9-108">**Bemærk:** Office-installation, der ofte opstår problemer forfalder til forkert konfigureret eller malformatted konfigurationsfiler.</span><span class="sxs-lookup"><span data-stu-id="a62d9-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="a62d9-109">For at undgå sådanne problemer, anbefaler vi, at du bruger Office Customization Tool til at oprette konfigurationsfilen.</span><span class="sxs-lookup"><span data-stu-id="a62d9-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="a62d9-110">Du kan også importere eksisterende konfigurationsfiler til Office-tilpasningsværktøjet.</span><span class="sxs-lookup"><span data-stu-id="a62d9-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="a62d9-111">Skift til den placering, hvor setup.exe er placeret fra en kommandoprompt og køre værktøjet Office installation i download-tilstand, og Angiv den konfigurationsfil, du lige har gemt.</span><span class="sxs-lookup"><span data-stu-id="a62d9-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="a62d9-112">I dette eksempel hedder konfigurationsfilen Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="a62d9-112">In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="a62d9-113">Kør værktøjet Office installation i konfigurere tilstand og angive konfigurationsfilen.</span><span class="sxs-lookup"><span data-stu-id="a62d9-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="a62d9-114">**Bemærk:** Fra den klientcomputer, hvor du vil installere Office, og du skal have lokale administratorrettigheder på denne computer, skal du udføre dette trin.</span><span class="sxs-lookup"><span data-stu-id="a62d9-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="a62d9-115">Hvis du vil vide mere om brugen af Office Deployment Tool for Office 365 ProPlus installationsscenarier, se [Oversigt over værktøjet Office installation](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="a62d9-115">To learn more about using Office Deployment Tool for your Office 365 ProPlus deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span></span> <span data-ttu-id="a62d9-116">Du kan finde flere oplysninger om, hvordan du bruger Office-tilpasningsværktøjet, [Oversigt over Office-tilpasningsværktøjet](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="a62d9-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
