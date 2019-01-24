---
title: Ved hjælp af værktøjet Office installation
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: b4ade0f21794a8986aa7a37d783da5fa289488fc
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/24/2019
ms.locfileid: "29463921"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="e6674-102">Ved hjælp af Office Deployment Tool (ODT)</span><span class="sxs-lookup"><span data-stu-id="e6674-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="e6674-p101">Du kan bruge Office Deployment Tool (ODT) til at installere Office 365-versioner af Office. Værktøjet Office installation (setup.exe) køres fra kommandolinjen og bruger en XML-konfigurationsfil til at bestemme, hvilke indstillinger der skal anvendes, når du installerer Office.</span><span class="sxs-lookup"><span data-stu-id="e6674-p101">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office. The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="e6674-105">Hent den nyeste version af værktøjet Office installation fra [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="e6674-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
    
2. <span data-ttu-id="e6674-p102">Brug [Office Customization Tool (OCT)](https://config.office.com) til at vælge dine indstillinger for installation og oprette XML-konfigurationsfilen. Eksportere konfigurationsfilen, og Placer den lokalt på den samme mappe, hvor setup.exe er placeret.</span><span class="sxs-lookup"><span data-stu-id="e6674-p102">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file. Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span> 
    
    <span data-ttu-id="e6674-p103">**Bemærk:** Office-installation, der ofte opstår problemer forfalder til forkert konfigureret eller malformatted konfigurationsfiler. For at undgå sådanne problemer, anbefaler vi, at du bruger Office Customization Tool til at oprette konfigurationsfilen. Du kan også importere eksisterende konfigurationsfiler til Office-tilpasningsværktøjet.</span><span class="sxs-lookup"><span data-stu-id="e6674-p103">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files. To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file. You can also import existing configuration files into the Office Customization Tool.</span></span> 
    
3. <span data-ttu-id="e6674-p104">Skift til den placering, hvor setup.exe er placeret fra en kommandoprompt og køre værktøjet Office installation i download-tilstand, og Angiv den konfigurationsfil, du lige har gemt. I dette eksempel hedder konfigurationsfilen Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="e6674-p104">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved. In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="e6674-113">Kør værktøjet Office installation i konfigurere tilstand og angive konfigurationsfilen.</span><span class="sxs-lookup"><span data-stu-id="e6674-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="e6674-114">**Bemærk:** Fra den klientcomputer, hvor du vil installere Office, og du skal have lokale administratorrettigheder på denne computer, skal du udføre dette trin.</span><span class="sxs-lookup"><span data-stu-id="e6674-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span> 
    
<span data-ttu-id="e6674-p105">Hvis du vil vide mere om brugen af Office Deployment Tool for Office 365 ProPlus installationsscenarier, se [Oversigt over værktøjet Office installation](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Du kan finde flere oplysninger om, hvordan du bruger Office-tilpasningsværktøjet, [Oversigt over Office-tilpasningsværktøjet](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="e6674-p105">To learn more about using Office Deployment Tool for your Office 365 ProPlus deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
  

