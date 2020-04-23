---
title: Sharepoint Online PowerShell
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 8c270748fc75f929371fbb2856daad3ae61a1540
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764255"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="7c62f-102">Sharepoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="7c62f-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="7c62f-103">Arbejder du med PowerShell eller Scripts i Sharepoint Online?</span><span class="sxs-lookup"><span data-stu-id="7c62f-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="7c62f-104">Besøg nedenstående links for mere information.</span><span class="sxs-lookup"><span data-stu-id="7c62f-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="7c62f-105">Introduktion til SharePoint Online Management Shell</span><span class="sxs-lookup"><span data-stu-id="7c62f-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="7c62f-106">Oprette forbindelse til SPO PowerShell med multifaktorgodkendelse (MFA)</span><span class="sxs-lookup"><span data-stu-id="7c62f-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="7c62f-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) indeholder et bibliotek med PowerShell-kommandoer, der giver dig mulighed for at udføre komplekse administrationshandlinger over for SPO.</span><span class="sxs-lookup"><span data-stu-id="7c62f-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="7c62f-108">Hvis du har problemer med at oprette forbindelse til SPO-administrationsshell, skal du kontrollere, at du har opdateret til den nyeste version, og forsøge at [importere modulet igen](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) ved hjælp af *"Import-Module Microsoft.Online.SharePoint.PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="7c62f-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="7c62f-109">Hvis du forsøger at køre objektmodelscripts på klientsiden, skal [sharepoint onlineklientkomponenterne sDK'et](https://www.microsoft.com/download/details.aspx?id=42038) være installeret på den lokale computer.</span><span class="sxs-lookup"><span data-stu-id="7c62f-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="7c62f-110">Hvis du har problemer med at køre scripts fra PowerShell, kan du overveje at køre PowerShell som administrator og ændre [kørselspolitikken](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="7c62f-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>