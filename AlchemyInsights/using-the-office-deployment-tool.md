---
title: Brug af Office-installationsværktøjet
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: fa40fef0de9b2e0e1fc329269c24e8bca9ed4146
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726242"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="da197-102">Bruge ODT (Office Deployment Tool)</span><span class="sxs-lookup"><span data-stu-id="da197-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="da197-103">Du kan bruge ODT (Office Deployment Tool) til at installere Office 365-versioner af Office.</span><span class="sxs-lookup"><span data-stu-id="da197-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="da197-104">Office Deployment Tool (setup.exe) køres fra kommandolinjen og bruger en XML-konfigurationsfil til at bestemme, hvilke indstillinger der skal anvendes ved installation af Office.</span><span class="sxs-lookup"><span data-stu-id="da197-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="da197-105">Hent den nyeste version af Office Deployment Tool fra [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="da197-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="da197-106">Brug [OKT (Office Customization Tool)](https://config.office.com) til at vælge installationsindstillingerne og oprette XML-konfigurationsfilen.</span><span class="sxs-lookup"><span data-stu-id="da197-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="da197-107">Eksporter konfigurationsfilen, og placer den lokalt i den samme mappe, hvor setup.exe er placeret.</span><span class="sxs-lookup"><span data-stu-id="da197-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="da197-108">**Bemærk:** Problemer med Office-installation opstår ofte på grund af forkert konfigurerede eller forkert formaterede konfigurationsfiler.</span><span class="sxs-lookup"><span data-stu-id="da197-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="da197-109">Hvis du vil undgå sådanne problemer, anbefales det, at du bruger Office-tilpasningsværktøjet til at oprette konfigurationsfilen.</span><span class="sxs-lookup"><span data-stu-id="da197-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="da197-110">Du kan også importere eksisterende konfigurationsfiler til Office-tilpasningsværktøjet.</span><span class="sxs-lookup"><span data-stu-id="da197-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="da197-111">Fra en kommandoprompt med en forhøjet kommando skal du skifte til den placering, hvor setup.exe er placeret, og køre Office-installationsværktøjet i overførselstilstand og angive den konfigurationsfil, du lige har gemt.</span><span class="sxs-lookup"><span data-stu-id="da197-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="da197-112">I dette eksempel hedder konfigurationsfilen Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="da197-112">In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="da197-113">Kør Office-installationsværktøjet i konfigureretilstand, og angiv konfigurationsfilen.</span><span class="sxs-lookup"><span data-stu-id="da197-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="da197-114">**Bemærk:** Du skal køre dette trin fra den klientcomputer, hvor du vil installere Office, og du skal have lokale administratortilladelser på den pågældende computer.</span><span class="sxs-lookup"><span data-stu-id="da197-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="da197-115">Hvis du vil have mere at vide om at bruge Office Deployment Tool til dine Microsoft 365 Apps til virksomhedsinstallationsscenarier, skal du se [Oversigt over Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="da197-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span></span> <span data-ttu-id="da197-116">Yderligere oplysninger om, hvordan du bruger Office-tilpasningsværktøjet, finder [du i Oversigt over Office-tilpasningsværktøjet](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="da197-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
