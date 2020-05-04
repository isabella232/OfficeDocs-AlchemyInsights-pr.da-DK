---
title: Installation af kontor på en Terminal Server - Uden licens
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 6e952513679c9ac66f8de2b43d6d243cf17ff789
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010608"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="1defc-102">Installere Office på en Terminal Server</span><span class="sxs-lookup"><span data-stu-id="1defc-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="1defc-103">Til installation af Microsoft 365 Apps til virksomheder på en Windows Server ved hjælp af RDS (Remote Desktop Services), der tidligere hed Terminal Services:</span><span class="sxs-lookup"><span data-stu-id="1defc-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="1defc-104">Du skal have et Microsoft 365-abonnement, der omfatter Microsoft 365 Apps til virksomheder, f.eks.</span><span class="sxs-lookup"><span data-stu-id="1defc-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="1defc-105">Microsoft 365 Apps til virksomheder og Microsoft 365 Apps til business Premium-planer omfatter ikke Microsoft 365 Apps til virksomheder.</span><span class="sxs-lookup"><span data-stu-id="1defc-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="1defc-106">Du skal aktivere [aktivering af delt computer](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="1defc-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="1defc-107">Hvis du vil installere Microsoft 365 Apps til virksomheder på RDS fra Microsoft 365 Administration, ***som bruger standardinstallationsindstillinger,*** skal du benytte følgende trin.</span><span class="sxs-lookup"><span data-stu-id="1defc-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="1defc-108">Du kan også hente og køre [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) for at installere Microsoft 365 Apps til virksomheder i aktiveringstilstand for delt computer.</span><span class="sxs-lookup"><span data-stu-id="1defc-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="1defc-109">Se, hvilket Microsoft 365-abonnement du har.</span><span class="sxs-lookup"><span data-stu-id="1defc-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="1defc-110">Lære</span><span class="sxs-lookup"><span data-stu-id="1defc-110">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="1defc-111">Skift om nødvendigt til et andet Microsoft 365-abonnement.</span><span class="sxs-lookup"><span data-stu-id="1defc-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="1defc-112">Lære</span><span class="sxs-lookup"><span data-stu-id="1defc-112">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="1defc-113">Hvis Office allerede er installeret på RDS-serveren ved hjælp af andre Microsoft 365-abonnementer, skal du fjerne det.</span><span class="sxs-lookup"><span data-stu-id="1defc-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="1defc-114">Ved at gå til \> Kontrolpanel Fjern et program.</span><span class="sxs-lookup"><span data-stu-id="1defc-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="1defc-115">Fjern ved hjælp af [Microsoft Support and Recovery Assistant,](https://aka.ms/SARA-OfficeUninstall-Alchemy) hvis du løber ind i problemer.</span><span class="sxs-lookup"><span data-stu-id="1defc-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="1defc-116">Log på Microsoft 365 Administration med din administratorkonto på RDS-serveren, og [installer Microsoft 365 Apps til virksomheder](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="1defc-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="1defc-117">Når Office er installeret, ***skal du ikke åbne eller logge på*** Office-programmer.</span><span class="sxs-lookup"><span data-stu-id="1defc-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="1defc-118">På RDS-serveren skal du aktivere delt computeraktivering ved at redigere registreringsdatabasen ved at følge disse trin:</span><span class="sxs-lookup"><span data-stu-id="1defc-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="1defc-119">Højreklik på Windows-knappen i nederste venstre hjørne af skærmen, og vælg Kør.</span><span class="sxs-lookup"><span data-stu-id="1defc-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="1defc-120">Skriv **regedit**i feltet Åbn , og vælg derefter OK.</span><span class="sxs-lookup"><span data-stu-id="1defc-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="1defc-121">Vælg Ja, når du bliver bedt om at tillade Registreringseditor at foretage ændringer på din enhed.</span><span class="sxs-lookup"><span data-stu-id="1defc-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="1defc-122">Tilføj en strengværdi af **SharedComputerLicensing** med en indstilling på 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration i Registreringseditor.</span><span class="sxs-lookup"><span data-stu-id="1defc-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="1defc-123">Log på som ***slutbruger på*** RDS-serveren, og [kontroller, at aktivering af den delte computer er aktiveret for Microsoft 365 Apps til virksomheder](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="1defc-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="1defc-124">Yderligere oplysninger om forudsætninger, installationsvejledning og vejledning i tilpassede installationer ved hjælp af Office Deployment Tool finder du under [Installere Microsoft 365 Apps til virksomheder ved hjælp af Fjernskrivebord-tjenester](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="1defc-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="1defc-125">Hvis du vil rette fejl i forbindelse med aktivering af delte computere, skal du se [Fejlfinding af problemer med aktivering af delt computer for Microsoft 365 Apps til virksomheder](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="1defc-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  