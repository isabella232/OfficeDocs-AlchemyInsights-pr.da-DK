---
title: Identificer problemer med virtuelt skrivebord i Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595514"
---
# <a name="identify-windows-virtual-desktop-issues"></a><span data-ttu-id="3e95c-102">Identificer problemer med virtuelt skrivebord i Windows</span><span class="sxs-lookup"><span data-stu-id="3e95c-102">Identify Windows Virtual Desktop issues</span></span>

<span data-ttu-id="3e95c-103">Windows Virtual Desktop Diagnostics bruger kun én PowerShell-cmdlet, men indeholder mange valgfrie parametre til at indskrænke og isolere problemer.</span><span class="sxs-lookup"><span data-stu-id="3e95c-103">Windows Virtual Desktop Diagnostics uses just one PowerShell cmdlet but contains many optional parameters to help narrow down and isolate issues.</span></span> <span data-ttu-id="3e95c-104">Sådan kommer du i gang:</span><span class="sxs-lookup"><span data-stu-id="3e95c-104">To get started:</span></span> 

1. <span data-ttu-id="3e95c-105">Download og importér Windows Virtual Desktop PowerShell-modulet.</span><span class="sxs-lookup"><span data-stu-id="3e95c-105">Download and import the Windows Virtual Desktop PowerShell module.</span></span> <span data-ttu-id="3e95c-106">Du kan finde flere oplysninger [i Windows Virtual Desktop Cmdlet'er til Windows PowerShell.](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)</span><span class="sxs-lookup"><span data-stu-id="3e95c-106">For details, see [Windows Virtual Desktop Cmdlets for Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span></span>

1. <span data-ttu-id="3e95c-107">Kør følgende cmdlet for at logge på din konto:</span><span class="sxs-lookup"><span data-stu-id="3e95c-107">Run the following cmdlet to sign in to your account:</span></span>
    
    <span data-ttu-id="3e95c-108">Eksempel: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span><span class="sxs-lookup"><span data-stu-id="3e95c-108">Example: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span></span>

<span data-ttu-id="3e95c-109">**BEMÆRK!** Alle forespørgsler, der bruger PowerShell, skal indeholde parametrene -UserName eller -ActivityID.</span><span class="sxs-lookup"><span data-stu-id="3e95c-109">**NOTE:** All queries using PowerShell must include either the -UserName or -ActivityID parameters.</span></span> <span data-ttu-id="3e95c-110">Du kan finde overvågningsegenskaber under [Brug Loganalyse til diagnosticeringsfunktionen.](https://go.microsoft.com/fwlink/?linkid=2126847)</span><span class="sxs-lookup"><span data-stu-id="3e95c-110">For monitoring capabilities, see Use [Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2126847).</span></span>

<span data-ttu-id="3e95c-111">Hvis du vil filtrere diagnosticeringsaktiviteter efter bruger, skal du køre følgende cmdlet:</span><span class="sxs-lookup"><span data-stu-id="3e95c-111">To filter diagnostic activities by user, run the following cmdlet:</span></span>

<span data-ttu-id="3e95c-112">Eksempel: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span><span class="sxs-lookup"><span data-stu-id="3e95c-112">Example: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span></span>

<span data-ttu-id="3e95c-113">Der er en liste over filtre, du kan køre for at diagnosticere problemer.</span><span class="sxs-lookup"><span data-stu-id="3e95c-113">There is a list of filters you can run to diagnose issues.</span></span> <span data-ttu-id="3e95c-114">Du kan få mere at vide om diagnosticering af problemer under [Identificere og diagnosticere problemer med virtuel skrivebord i Windows.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)</span><span class="sxs-lookup"><span data-stu-id="3e95c-114">To learn more about diagnosing issues, see [Identify and diagnose Windows Virtual Desktop issues](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span></span>

<span data-ttu-id="3e95c-115">Hvis du vil have mere at vide om almindelige fejl, skal du se Almindelige fejl [senarios.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios)</span><span class="sxs-lookup"><span data-stu-id="3e95c-115">To learn more about common errors, see [Common errors senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span></span>
