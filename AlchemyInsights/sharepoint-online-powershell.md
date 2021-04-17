---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 839a70282b4dd619e9dbe8167ef0e409e468b1ad
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830576"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="41930-102">Sharepoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="41930-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="41930-103">Arbejder du med PowerShell eller scripts i Sharepoint Online?</span><span class="sxs-lookup"><span data-stu-id="41930-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="41930-104">Besøg nedenstående links for at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="41930-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="41930-105">Introduktion til SharePoint Online Management Shell</span><span class="sxs-lookup"><span data-stu-id="41930-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="41930-106">Opret forbindelse til SPO PowerShell med multifaktorgodkendelse (MFA)</span><span class="sxs-lookup"><span data-stu-id="41930-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="41930-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) indeholder et bibliotek af PowerShell-kommandoer, der gør det muligt at udføre komplekse administrationshandlinger i forbindelse med SPO.</span><span class="sxs-lookup"><span data-stu-id="41930-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="41930-108">Hvis du har problemer med at oprette forbindelse til SPO management shell, skal [](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) du kontrollere, at du har opdateret til den nyeste version og prøve at importere modulet igen ved hjælp af *"Import-Module Microsoft.Online.SharePoint.PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="41930-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="41930-109">Hvis du forsøger at køre scripts til objektmodeller på klientsiden, skal [SDK'en til Sharepoint](https://www.microsoft.com/download/details.aspx?id=42038) Online-klientkomponenter være installeret på din lokale computer.</span><span class="sxs-lookup"><span data-stu-id="41930-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="41930-110">Hvis du har problemer med at køre scripts fra PowerShell, kan du overveje at køre PowerShell som administrator og ændre [eksekveringspolitikken.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)</span><span class="sxs-lookup"><span data-stu-id="41930-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>