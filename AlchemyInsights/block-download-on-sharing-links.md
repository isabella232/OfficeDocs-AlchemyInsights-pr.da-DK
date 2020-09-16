---
title: Bloker hentning af delingslinks
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000213"
- "5715"
ms.openlocfilehash: 5837013a71648d5d53cd215c3e3489f3de5528d5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685736"
---
# <a name="block-download-on-sharing-links"></a><span data-ttu-id="022cd-102">Bloker hentning af delingslinks</span><span class="sxs-lookup"><span data-stu-id="022cd-102">Block download on sharing links</span></span>

<span data-ttu-id="022cd-103">**Bloker hentning** er tilgængelig for **skrivebeskyttede links** til Office-dokumenter.</span><span class="sxs-lookup"><span data-stu-id="022cd-103">**Block download** is available for **view-only links** to Office documents.</span></span> <span data-ttu-id="022cd-104">Når du vælger denne indstilling, kan personer, der får adgang til filen via det link, du har oprettet, ikke se muligheder for at hente, udskrive eller kopiere filen.</span><span class="sxs-lookup"><span data-stu-id="022cd-104">When you select this option, people who gain access to the file via the link you created will not see options to download, print, or copy the file.</span></span>

<span data-ttu-id="022cd-105">Administratorer kan kontrollere, om indstillingen "Bloker hentning af filer" kun vises for Office-filer eller ej ved at ændre `BlockDownloadLinksFileType` indstillingen i PowerShell [-cmdlet'en Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) eller [set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="022cd-105">Administrators can control whether the "block download" setting appears only for Office files or not by changing the `BlockDownloadLinksFileType` setting in the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) or [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell cmdlets.</span></span>
