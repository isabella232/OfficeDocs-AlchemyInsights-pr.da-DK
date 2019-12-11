---
title: Implementering af Office 365 ProPlus til delt brug på RDS, Terminal Server eller VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959454"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="5c233-102">Implementering af Office 365 ProPlus til delt brug på RDS, Terminal Server eller VDI</span><span class="sxs-lookup"><span data-stu-id="5c233-102">Deploying Office 365 ProPlus for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="5c233-103">Sådan implementeres Office 365 ProPlus ved hjælp af RDS (Remote Desktop Services), der tidligere hed Terminal Services:</span><span class="sxs-lookup"><span data-stu-id="5c233-103">To deploy Office 365 ProPlus using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
- <span data-ttu-id="5c233-104">Du skal have en Microsoft 365 for business-plan eller en Office 365-plan, der omfatter Office 365 ProPlus, såsom Office 365 Enterprise E3 eller Enterprise e5.</span><span class="sxs-lookup"><span data-stu-id="5c233-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE] 
   > <span data-ttu-id="5c233-105">Office 365 Business-og Office 365 Business Premium-planerne indeholder ikke Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="5c233-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
- <span data-ttu-id="5c233-106">Du skal aktivere [Aktivering af delt computer](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="5c233-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

> [!NOTE]
> <span data-ttu-id="5c233-107">Du kan også hente og køre [Microsofts support-og genoprettelsesassistent](https://aka.ms/SaRA_OfficeSCA_M365Portal) for at installere Office 365 ProPlus i den delte computer aktiveringstilstand.</span><span class="sxs-lookup"><span data-stu-id="5c233-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Office 365 ProPlus in shared computer activation mode.</span></span>

<span data-ttu-id="5c233-108">Du finder flere oplysninger om forudsætninger, installationsvejledninger og vejledning om tilpassede installationer ved hjælp af Office-installationsværktøjet under [implementere office 365 ProPlus ved hjælp af Fjernskrivebord-tjenester](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="5c233-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>

<span data-ttu-id="5c233-109">Sådan rettes fejl i forbindelse med aktivering af delt computer:</span><span class="sxs-lookup"><span data-stu-id="5c233-109">To fix errors related to shared computer activation:</span></span>
- <span data-ttu-id="5c233-110">Se [fejlfinding af problemer med delt computeraktivering for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="5c233-110">See [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
- <span data-ttu-id="5c233-111">Se [Nulstil Office 365 ProPlus-aktiveringstilstand](https://go.microsoft.com/fwlink/?linkid=2109218).</span><span class="sxs-lookup"><span data-stu-id="5c233-111">See [Reset Office 365 ProPlus activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="5c233-112">Hvis du vil installere Office 365 ProPlus på RDS fra Microsoft 365 administration, ***som bruger standardindstillinger for installation***, skal du benytte følgende fremgangsmåde:</span><span class="sxs-lookup"><span data-stu-id="5c233-112">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1.  <span data-ttu-id="5c233-113">Tjek, hvad Office 365 plan du har.</span><span class="sxs-lookup"><span data-stu-id="5c233-113">Check what Office 365 plan you have.</span></span> <span data-ttu-id="5c233-114">[Lær hvordan](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).</span><span class="sxs-lookup"><span data-stu-id="5c233-114">[Learn how](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2.  <span data-ttu-id="5c233-115">Skift om nødvendigt til en anden Office 365-plan.</span><span class="sxs-lookup"><span data-stu-id="5c233-115">If necessary, switch to a different Office 365 plan.</span></span> <span data-ttu-id="5c233-116">[Lær hvordan](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span><span class="sxs-lookup"><span data-stu-id="5c233-116">[Learn how](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span></span>
3.  <span data-ttu-id="5c233-117">Hvis Office allerede er installeret på RDS-serveren ved hjælp af andre Office 365-planer, skal du afinstallere det.</span><span class="sxs-lookup"><span data-stu-id="5c233-117">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="5c233-118">For eksempel ved at gå til **kontrol panel** > **afinstallere et program**.</span><span class="sxs-lookup"><span data-stu-id="5c233-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="5c233-119">Afinstaller ved hjælp af [Microsofts support-og genoprettelsesassistent](https://aka.ms/SARA-OfficeUninstall-Alchemy) , hvis du løber ind i problemer.</span><span class="sxs-lookup"><span data-stu-id="5c233-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4.  <span data-ttu-id="5c233-120">På RDS-serveren skal du logge på Microsoft 365 administration med din administratorkonto og [installere Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="5c233-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5.  <span data-ttu-id="5c233-121">Når Office er installeret, skal ***du ikke åbne eller logge*** på nogen Office-programmer.</span><span class="sxs-lookup"><span data-stu-id="5c233-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6.  <span data-ttu-id="5c233-122">Aktivér aktivering af delt computer på RDS-serveren ved at redigere registreringsdatabasen ved at følge disse trin:</span><span class="sxs-lookup"><span data-stu-id="5c233-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="5c233-123">Højreklik på Windows-knappen i nederste venstre hjørne af skærmen, og vælg **Kør**.</span><span class="sxs-lookup"><span data-stu-id="5c233-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="5c233-124">Skriv **regedit**i feltet Åbn, og vælg derefter **OK**.</span><span class="sxs-lookup"><span data-stu-id="5c233-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="5c233-125">Vælg **Ja** , når du bliver bedt om at tillade registrerings Editor at foretage ændringer på din enhed.</span><span class="sxs-lookup"><span data-stu-id="5c233-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="5c233-126">Tilføj en strengværdi af **Sharedcomputerlicensing** i registreringseditoren med en indstilling på 1 under HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="5c233-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="5c233-127">***Log på som en slutbruger*** på RDS-serveren, og [Bekræft, at aktivering af den delte computer er aktiveret for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="5c233-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

