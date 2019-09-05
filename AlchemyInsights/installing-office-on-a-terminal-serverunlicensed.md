---
title: Installation af Office på en Terminal Server-uden licens
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 53071224a7c33532d864cd70b84bf0e3cc6a992f
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/04/2019
ms.locfileid: "36735383"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="3a751-102">Installere Office på en Terminal Server</span><span class="sxs-lookup"><span data-stu-id="3a751-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="3a751-103">Til installation af Office 365 ProPlus på en Windows-Server ved hjælp af RDS (Remote Desktop Services), der tidligere hed Terminal Services:</span><span class="sxs-lookup"><span data-stu-id="3a751-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="3a751-104">Du skal have en Office 365-plan, der omfatter Office 365 ProPlus, f. eks Office 365 Enterprise E3 eller Enterprise e5.</span><span class="sxs-lookup"><span data-stu-id="3a751-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="3a751-105">Office 365 Business-og Office 365 Business Premium-planerne indeholder ikke Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="3a751-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="3a751-106">Du skal aktivere [delt computeraktivering](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="3a751-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="3a751-107">Hvis du vil installere Office 365 ProPlus på RDS fra Microsoft 365 administration, ***som bruger standardindstillinger for installation***, skal du følge disse trin:</span><span class="sxs-lookup"><span data-stu-id="3a751-107">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, follow these steps:</span></span>
  
1. <span data-ttu-id="3a751-108">Tjek, hvad Office 365 plan du har.</span><span class="sxs-lookup"><span data-stu-id="3a751-108">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="3a751-109">Lære</span><span class="sxs-lookup"><span data-stu-id="3a751-109">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="3a751-110">Skift om nødvendigt til en anden Office 365-plan.</span><span class="sxs-lookup"><span data-stu-id="3a751-110">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="3a751-111">Lære</span><span class="sxs-lookup"><span data-stu-id="3a751-111">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="3a751-112">Hvis Office allerede er installeret på RDS-serveren ved hjælp af andre Office 365-planer, skal du afinstallere det.</span><span class="sxs-lookup"><span data-stu-id="3a751-112">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="3a751-113">For eksempel ved at gå til kontrol panel \> afinstallere et program.</span><span class="sxs-lookup"><span data-stu-id="3a751-113">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="3a751-114">Afinstaller ved hjælp af [Microsofts support-og genoprettelsesassistent](https://aka.ms/SARA-OfficeUninstall-Alchemy) , hvis du løber ind i problemer.</span><span class="sxs-lookup"><span data-stu-id="3a751-114">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="3a751-115">På RDS-serveren skal du logge på Microsoft 365 administration med din administratorkonto og [installere Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="3a751-115">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="3a751-116">Når Office er installeret, skal ***du ikke åbne eller logge*** på nogen Office-programmer.</span><span class="sxs-lookup"><span data-stu-id="3a751-116">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="3a751-117">Aktivér aktivering af delt computer på RDS-serveren ved at redigere registreringsdatabasen ved at følge disse trin:</span><span class="sxs-lookup"><span data-stu-id="3a751-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="3a751-118">Højreklik på Windows-knappen i nederste venstre hjørne af skærmen, og vælg Kør.</span><span class="sxs-lookup"><span data-stu-id="3a751-118">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="3a751-119">Skriv **regedit**i feltet Åbn, og vælg derefter OK.</span><span class="sxs-lookup"><span data-stu-id="3a751-119">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="3a751-120">Vælg Ja, når du bliver bedt om at tillade registrerings Editor at foretage ændringer på din enhed.</span><span class="sxs-lookup"><span data-stu-id="3a751-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="3a751-121">Tilføj en strengværdi af **Sharedcomputerlicensing** i registreringseditoren med en indstilling på 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="3a751-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="3a751-122">***Log på som en slutbruger*** på RDS-serveren, og [Bekræft, at aktivering af den delte computer er aktiveret for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="3a751-122">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="3a751-123">Du kan finde flere oplysninger om forudsætninger, installationsvejledninger og vejledning om tilpassede installationer ved hjælp af Office-installationsværktøjet under [installere office 365 ProPlus ved hjælp af Fjernskrivebord-tjenester](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="3a751-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="3a751-124">Hvis du vil rette fejl i forbindelse med aktivering af delt computer, skal du se [fejlfinding af problemer med delt computeraktivering for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="3a751-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  