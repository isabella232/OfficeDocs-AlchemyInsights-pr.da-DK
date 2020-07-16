---
title: Problemer med Yammer-licenser
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148201"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="02870-102">Problemer med Yammer-licenser</span><span class="sxs-lookup"><span data-stu-id="02870-102">Yammer licensing issues</span></span>

<span data-ttu-id="02870-103">Alle brugere skal have licens til at bruge Yammer Enterprise-tjenesten, men Yammer kræver som standard ikke, at brugerne har licens til at få adgang til tjenesten.</span><span class="sxs-lookup"><span data-stu-id="02870-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="02870-104">Når en administrator ændrer indstillingen for at blokere Microsoft 365-brugere uden Yammer-licenser, kan brugere, der ikke har fået tildelt en Yammer Enterprise-licens, ikke få adgang til Yammer-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="02870-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="02870-105">Du kan finde flere oplysninger under [Administrere Yammer-brugerlicenser i Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="02870-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="02870-106">Når licenser fjernes fra brugere, vises Yammer-feltet ikke længere, og andre tjenester kan bruge fjernelse af licenser til at skjule funktioner.</span><span class="sxs-lookup"><span data-stu-id="02870-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="02870-107">I andre tilfælde kan funktioner stadig vises, men kræver licenstildeling for at fungere.</span><span class="sxs-lookup"><span data-stu-id="02870-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="02870-108">**Licensen opdateres ikke for brugeren**</span><span class="sxs-lookup"><span data-stu-id="02870-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="02870-109">Af og til tildeles en bruger en licens, men kan stadig ikke få adgang til Yammer.</span><span class="sxs-lookup"><span data-stu-id="02870-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="02870-110">Der er større sandsynlighed for forsinkelser, når en masselicenstildeling er i gang.</span><span class="sxs-lookup"><span data-stu-id="02870-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="02870-111">Yammer-brugere opdateres muligvis ikke i samme rækkefølge, som licenser ændres i Azure AD, fordi systemet kører asynkront.</span><span class="sxs-lookup"><span data-stu-id="02870-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="02870-112">Vent op til 24 timer, før du åbner en supportsag for at rapportere licenssynkroniseringsproblemer.</span><span class="sxs-lookup"><span data-stu-id="02870-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="02870-113">**Masselicenstildeling**</span><span class="sxs-lookup"><span data-stu-id="02870-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="02870-114">Licenser kan tildeles via Administration eller PowerShell-scripting.</span><span class="sxs-lookup"><span data-stu-id="02870-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="02870-115">Du kan finde flere oplysninger under [Tildele licenser til brugere](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) og Tildele licenser til [brugerkonti med Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="02870-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="02870-116">Microsoft Support hjælper ikke med at oprette scripts, men dokumentation om Yammer-licenstildeling er tilgængelig.</span><span class="sxs-lookup"><span data-stu-id="02870-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="02870-117">Du kan finde flere oplysninger under [Administrere Yammer-licenser ved hjælp af Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="02870-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>