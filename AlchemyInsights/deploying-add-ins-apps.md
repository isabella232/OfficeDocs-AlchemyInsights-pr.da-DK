---
title: Installation af tilføjelsesprogrammet til Microsoft 365 Apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: e55d8e5453f60b5993500dae1eb6efce11a8aa1a
ms.sourcegitcommit: d74039304002e526ba6f8ca02e76e4ce7e1aa743
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/30/2021
ms.locfileid: "52124965"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="6aeb8-102">Installation af tilføjelsesprogrammet til Microsoft 365 Apps</span><span class="sxs-lookup"><span data-stu-id="6aeb8-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="6aeb8-103">Centraliseret udrulning er den anbefalede metode til Office udrulning af tilføjelsesprogrammet til brugere og grupper i organisationen.</span><span class="sxs-lookup"><span data-stu-id="6aeb8-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="6aeb8-104">Hvis du vil installere tilføjelsesprogrammet, skal du følge nedenstående trin:</span><span class="sxs-lookup"><span data-stu-id="6aeb8-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="6aeb8-105">**Bemærk!** Hvis du vil installere tilføjelsesprogrammer til Office som individuel bruger, skal du se Få vist, administrer og installér tilføjelsesprogrammer [i Office programmer.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)</span><span class="sxs-lookup"><span data-stu-id="6aeb8-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="6aeb8-106">Sørg også for, at individuel anskaffelse af Office Store er aktiveret.</span><span class="sxs-lookup"><span data-stu-id="6aeb8-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> 

1. <span data-ttu-id="6aeb8-107">Sørg for, at dit miljø opfylder kravene til udrulning af tilføjelser ved hjælp af Centraliseret udrulning.</span><span class="sxs-lookup"><span data-stu-id="6aeb8-107">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="6aeb8-108">Du kan få mere at vide under [Krav](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span><span class="sxs-lookup"><span data-stu-id="6aeb8-108">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="6aeb8-109">Gå til **Indstillinger**  >  **integrerede apps** Hent  >  **apps** i Microsoft 365 Administration for at installere tilføjelsesprogrammer.</span><span class="sxs-lookup"><span data-stu-id="6aeb8-109">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="6aeb8-110">Bemærkninger:</span><span class="sxs-lookup"><span data-stu-id="6aeb8-110">Notes:</span></span> 

- <span data-ttu-id="6aeb8-111">Integrerede apps kræver, at administratoren har globale administrator- Exchange administratortilladelser.</span><span class="sxs-lookup"><span data-stu-id="6aeb8-111">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="6aeb8-112">Når du installerer tilføjelser til flere brugere, anbefaler vi, at du foretager tildelinger ved hjælp af grupper i stedet for individuelle brugere.</span><span class="sxs-lookup"><span data-stu-id="6aeb8-112">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="6aeb8-113">Du kan få mere at [vide under Overvejelser ved tildeling af et tilføjelsesprogrammet til brugere og grupper.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)</span><span class="sxs-lookup"><span data-stu-id="6aeb8-113">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="6aeb8-114">Centraliseret udrulning understøtter ikke brugere i indlejrede grupper eller grupper, der har overordnede grupper.</span><span class="sxs-lookup"><span data-stu-id="6aeb8-114">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="6aeb8-115">Du kan få mere at [vide under Bruger- og gruppetildelinger.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)</span><span class="sxs-lookup"><span data-stu-id="6aeb8-115">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="6aeb8-116">Sørg for, at Microsoft 365 GUID (App Management Service: '0517ffae-825d-4aff-999e-3f2336b8a20a') er aktiveret til at logge på.</span><span class="sxs-lookup"><span data-stu-id="6aeb8-116">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="6aeb8-117">Du kan få mere at vide [under Konfigurere appegenskaber](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span><span class="sxs-lookup"><span data-stu-id="6aeb8-117">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="6aeb8-118">Hvis du oplever problemer med installation af tilføjelsesprogrammer ved hjælp af integrerede apps, kan du prøve at [installere ved hjælp af tilføjelsesprogrammer](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span><span class="sxs-lookup"><span data-stu-id="6aeb8-118">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="6aeb8-119">Du kan finde flere oplysninger under:</span><span class="sxs-lookup"><span data-stu-id="6aeb8-119">For more information, see:</span></span>

<span data-ttu-id="6aeb8-120">[Installér tilføjelser i Administration](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Administrer tilføjelser i Administration](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Brug de Centraliserede udrulning af PowerShell-cmdlet'er til at administrere tilføjelsesinstallationer](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Publicere Office-tilføjelsesprogrammet ved hjælp af Centraliseret udrulning via Microsoft 365 Administration](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Fejlfinding: Brugeren kan ikke se tilføjelsesprogram](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Fejlfinding af brugerfejl Office tilføjelsesprogram](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="6aeb8-120">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>