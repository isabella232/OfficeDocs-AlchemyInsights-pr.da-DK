---
title: Installationen af office på en Terminal Server - uden licens
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 971edd9c064b448446ba16361e99df4a2291c14f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/23/2019
ms.locfileid: "32410116"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="f70e6-102">Installationen af Office på en Terminal Server</span><span class="sxs-lookup"><span data-stu-id="f70e6-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="f70e6-103">Til implementering af Office 365 ProPlus på en Windows-Server ved hjælp af Remote Desktop Services (RDS), tidligere kaldet Terminal Services:</span><span class="sxs-lookup"><span data-stu-id="f70e6-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="f70e6-104">Du skal have en Office 365-plan, der indeholder Office 365 ProPlus, som Office 365 Enterprise E3 eller Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="f70e6-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="f70e6-105">Business til Office 365 og Office 365 Business Premium planerne indeholder ikke Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="f70e6-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
    
- <span data-ttu-id="f70e6-106">Du skal aktivere [delt computeraktivering](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="f70e6-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>
    
<span data-ttu-id="f70e6-107">Hvis du vil installere Office 365 ProPlus på RDS fra Office 365-portalen, \*\* *som bruger standardindstillingerne for installation* \*\*, skal du følge disse trin:</span><span class="sxs-lookup"><span data-stu-id="f70e6-107">If you want to install Office 365 ProPlus on RDS from the Office 365 portal, \*\* *which uses default installation settings* \*\*, follow these steps:</span></span> 
  
1. <span data-ttu-id="f70e6-108">Kontrollere, hvilke Office 365-plan, du har.</span><span class="sxs-lookup"><span data-stu-id="f70e6-108">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="f70e6-109">Lær, hvordan</span><span class="sxs-lookup"><span data-stu-id="f70e6-109">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
    
2. <span data-ttu-id="f70e6-110">Hvis nødvendigt, Skift til en anden Office 365-planer.</span><span class="sxs-lookup"><span data-stu-id="f70e6-110">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="f70e6-111">Lær, hvordan</span><span class="sxs-lookup"><span data-stu-id="f70e6-111">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
    
3. <span data-ttu-id="f70e6-112">Hvis Office er allerede installeret på RDS-serveren ved hjælp af andre Office 365-planer, kan du fjerne den.</span><span class="sxs-lookup"><span data-stu-id="f70e6-112">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="f70e6-113">For eksempel ved at gå til Kontrolpanel \> afinstallerer et program.</span><span class="sxs-lookup"><span data-stu-id="f70e6-113">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="f70e6-114">Fjern ved hjælp af [Microsoft Support og genoprettelse-assistenten](https://aka.ms/SARA-OfficeUninstall-Alchemy) , hvis du kører i problemer.</span><span class="sxs-lookup"><span data-stu-id="f70e6-114">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span> 
    
4. <span data-ttu-id="f70e6-115">Log på Office 365-portalen med administratorkonto og [installere Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx)på RDS-serveren.</span><span class="sxs-lookup"><span data-stu-id="f70e6-115">On the RDS server, sign in to the Office 365 portal with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
    
5. <span data-ttu-id="f70e6-116">Når Office er installeret, \*\* *ikke åbne eller logge på* \*\* til Office-programmer.</span><span class="sxs-lookup"><span data-stu-id="f70e6-116">After Office is installed, \*\* *don't open or sign in* \*\* to any Office applications.</span></span> 
    
6. <span data-ttu-id="f70e6-117">Aktiver delt computeraktivering på RDS-serveren, ved at redigere registreringsdatabasen ved at følge disse trin:</span><span class="sxs-lookup"><span data-stu-id="f70e6-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
    
1. <span data-ttu-id="f70e6-118">Højreklik på Windows-knappen i nederste venstre hjørne af skærmen og Vælg Kør.</span><span class="sxs-lookup"><span data-stu-id="f70e6-118">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="f70e6-119">Skriv **regedit**i boksen Åbn, og klik derefter på OK.</span><span class="sxs-lookup"><span data-stu-id="f70e6-119">In the Open box, type **regedit**, and then select OK.</span></span> 
    
2. <span data-ttu-id="f70e6-120">Vælg Ja, når du bliver bedt om at tillade Registreringseditor til at foretage ændringer til din enhed.</span><span class="sxs-lookup"><span data-stu-id="f70e6-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>
    
3. <span data-ttu-id="f70e6-121">I Registreringseditor, føje en strengværdi af **SharedComputerLicensing** med indstillingen 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="f70e6-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span> 
    
7. <span data-ttu-id="f70e6-122">På RDS-serveren \*\* *logge på som en slutbruger* \*\*, og [Kontroller, at aktivering af delt computer aktiveres for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="f70e6-122">On the RDS server, \*\* *sign in as an end user* \*\* and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>
    
<span data-ttu-id="f70e6-123">Yderligere oplysninger om forudsætninger, installationsvejledning og vejledning om tilpassede installationer ved hjælp af værktøjet Office installation, finder du [Installere Office 365 ProPlus ved hjælp af Fjernskrivebord-tjenester](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="f70e6-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="f70e6-124">For at rette fejl, der er relateret til aktivering af delt computer, se [fejlfinding i forbindelse med problemer med aktivering af delt computer til Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="f70e6-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  

