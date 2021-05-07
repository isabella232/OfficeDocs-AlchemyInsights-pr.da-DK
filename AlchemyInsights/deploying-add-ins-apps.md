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
ms.openlocfilehash: a878a35ba9b530ce22ca7c263d20bd942d6896a8
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233514"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="7ca60-102">Installation af tilføjelsesprogrammet til Microsoft 365 Apps</span><span class="sxs-lookup"><span data-stu-id="7ca60-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="7ca60-103">Centraliseret udrulning er den anbefalede metode til Office udrulning af tilføjelsesprogrammet til brugere og grupper i organisationen.</span><span class="sxs-lookup"><span data-stu-id="7ca60-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="7ca60-104">Hvis du vil installere tilføjelsesprogrammet, skal du følge nedenstående trin:</span><span class="sxs-lookup"><span data-stu-id="7ca60-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="7ca60-105">**Bemærk!** Hvis du vil installere tilføjelsesprogrammer til Office som individuel bruger, skal du se Få vist, administrer og installér tilføjelsesprogrammer [i Office programmer.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)</span><span class="sxs-lookup"><span data-stu-id="7ca60-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="7ca60-106">Sørg også for, at individuel anskaffelse af Office Store er aktiveret.</span><span class="sxs-lookup"><span data-stu-id="7ca60-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> <span data-ttu-id="7ca60-107">Du kan få mere at vide under Undgå downloads af tilføjelsesprogrammet ved at deaktivere Office Store på tværs af alle [klienter (undtagen Outlook).](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook)</span><span class="sxs-lookup"><span data-stu-id="7ca60-107">For details, see [Prevent add-in downloads by turning off the Office Store across all clients (Except Outlook)](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook).</span></span>

1. <span data-ttu-id="7ca60-108">Sørg for, at dit miljø opfylder kravene til udrulning af tilføjelser ved hjælp af Centraliseret udrulning.</span><span class="sxs-lookup"><span data-stu-id="7ca60-108">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="7ca60-109">Du kan få mere at vide under [Krav](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span><span class="sxs-lookup"><span data-stu-id="7ca60-109">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="7ca60-110">Gå til **Indstillinger**  >  **integrerede apps** Hent  >  **apps** i Microsoft 365 Administration for at installere tilføjelsesprogrammer.</span><span class="sxs-lookup"><span data-stu-id="7ca60-110">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="7ca60-111">Bemærkninger:</span><span class="sxs-lookup"><span data-stu-id="7ca60-111">Notes:</span></span> 

- <span data-ttu-id="7ca60-112">Integrerede apps kræver, at administratoren har globale administrator- Exchange administratortilladelser.</span><span class="sxs-lookup"><span data-stu-id="7ca60-112">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="7ca60-113">Når du installerer tilføjelser til flere brugere, anbefaler vi, at du foretager tildelinger ved hjælp af grupper i stedet for individuelle brugere.</span><span class="sxs-lookup"><span data-stu-id="7ca60-113">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="7ca60-114">Du kan få mere at [vide under Overvejelser ved tildeling af et tilføjelsesprogrammet til brugere og grupper.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)</span><span class="sxs-lookup"><span data-stu-id="7ca60-114">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="7ca60-115">Centraliseret udrulning understøtter ikke brugere i indlejrede grupper eller grupper, der har overordnede grupper.</span><span class="sxs-lookup"><span data-stu-id="7ca60-115">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="7ca60-116">Du kan få mere at [vide under Bruger- og gruppetildelinger.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)</span><span class="sxs-lookup"><span data-stu-id="7ca60-116">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="7ca60-117">Sørg for, at Microsoft 365 GUID (App Management Service: '0517ffae-825d-4aff-999e-3f2336b8a20a') er aktiveret til at logge på.</span><span class="sxs-lookup"><span data-stu-id="7ca60-117">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="7ca60-118">Du kan få mere at vide [under Konfigurere appegenskaber](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span><span class="sxs-lookup"><span data-stu-id="7ca60-118">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="7ca60-119">Hvis du oplever problemer med installation af tilføjelsesprogrammer ved hjælp af integrerede apps, kan du prøve at [installere ved hjælp af tilføjelsesprogrammer](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span><span class="sxs-lookup"><span data-stu-id="7ca60-119">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="7ca60-120">Du kan finde flere oplysninger under:</span><span class="sxs-lookup"><span data-stu-id="7ca60-120">For more information, see:</span></span>

<span data-ttu-id="7ca60-121">[Installér tilføjelser i Administration](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Administrer tilføjelser i Administration](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Brug de Centraliserede udrulning af PowerShell-cmdlet'er til at administrere tilføjelsesinstallationer](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Publicere Office-tilføjelsesprogrammet ved hjælp af Centraliseret udrulning via Microsoft 365 Administration](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Fejlfinding: Brugeren kan ikke se tilføjelsesprogram](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Fejlfinding af brugerfejl Office tilføjelsesprogram](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="7ca60-121">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>