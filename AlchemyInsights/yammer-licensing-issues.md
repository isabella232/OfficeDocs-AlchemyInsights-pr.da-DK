---
title: Problemer med Yammer-licens
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657270"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="0ac18-102">Problemer med Yammer-licens</span><span class="sxs-lookup"><span data-stu-id="0ac18-102">Yammer licensing issues</span></span>

<span data-ttu-id="0ac18-103">Alle brugere skal have en licens for at bruge Yammer Enterprise-tjenesten, men som standard kræver Yammer ikke, at brugere har en licens til at få adgang til tjenesten.</span><span class="sxs-lookup"><span data-stu-id="0ac18-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="0ac18-104">Når en administrator ændrer indstillingen for at blokere Microsoft 365-brugere uden Yammer-licenser, har brugere, der ikke har fået tildelt en Yammer Enterprise-licens, ikke adgang til Yammer-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="0ac18-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="0ac18-105">Du kan finde flere oplysninger i [administrere Yammer-brugerlicenser i Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="0ac18-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="0ac18-106">Når licenser fjernes fra brugerne, vises Yammer-feltet ikke længere, og andre tjenester kan bruge Fjern licens til at skjule funktioner.</span><span class="sxs-lookup"><span data-stu-id="0ac18-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="0ac18-107">I andre tilfælde kan funktioner stadig vises, men kræver licenstildeling for at fungere.</span><span class="sxs-lookup"><span data-stu-id="0ac18-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="0ac18-108">**Licensen bliver ikke opdateret for brugeren**</span><span class="sxs-lookup"><span data-stu-id="0ac18-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="0ac18-109">Nogle gange tildeles en bruger en licens, men det er stadig ikke muligt at få adgang til Yammer.</span><span class="sxs-lookup"><span data-stu-id="0ac18-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="0ac18-110">Der er større sandsynlighed for forsinkelser, når der er en masse licenstildeling i gang.</span><span class="sxs-lookup"><span data-stu-id="0ac18-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="0ac18-111">Yammer-brugere opdateres muligvis ikke i samme rækkefølge, da licenser er ændret i Azure AD, fordi systemet kører asynkront.</span><span class="sxs-lookup"><span data-stu-id="0ac18-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="0ac18-112">Vent op til 24 timer, før du åbner en support situation for at rapportere problemer med synkronisering af licenser.</span><span class="sxs-lookup"><span data-stu-id="0ac18-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="0ac18-113">**Masse licenstildeling**</span><span class="sxs-lookup"><span data-stu-id="0ac18-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="0ac18-114">Licenser kan tildeles via Administrationscenter eller PowerShell-scripting.</span><span class="sxs-lookup"><span data-stu-id="0ac18-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="0ac18-115">Du kan få mere at vide under [Tildel licenser til brugere](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) og [Tildel licenser til brugerkonti med Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="0ac18-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="0ac18-116">Microsoft Support yder ikke hjælp til oprettelse af scripts, men dokumentation til Yammer-licenstildeling er tilgængelig.</span><span class="sxs-lookup"><span data-stu-id="0ac18-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="0ac18-117">Du kan finde flere oplysninger i [administrere Yammer-licenser ved hjælp af Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="0ac18-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>