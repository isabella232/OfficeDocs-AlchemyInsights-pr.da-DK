---
title: Problemer med SharePoint Designer-forbindelse
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 01ccc6bc28148f397fb6cd2b7a0eaaeb5b51973f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511538"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="92541-102">Problemer med SharePoint Designer-forbindelse</span><span class="sxs-lookup"><span data-stu-id="92541-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="92541-103">Hvis SharePoint Designer oplever forbindelsesproblemer til SharePoint-websteder, skal du prøve følgende almindelige løsninger.</span><span class="sxs-lookup"><span data-stu-id="92541-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="92541-104">Trin 1: Kontroller, at SharePoint Designer 2013 er opdateret med [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) og [den 2.](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)</span><span class="sxs-lookup"><span data-stu-id="92541-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="92541-105">Trin 2: Ryd de lokale cachefiler:</span><span class="sxs-lookup"><span data-stu-id="92541-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="92541-106">Luk SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="92541-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="92541-107">Fjern alle filer, der findes i hver af følgende mapper, på den lokale computer.</span><span class="sxs-lookup"><span data-stu-id="92541-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="92541-108">%APPDATA%\Microsoft\WebServerudvidelser\Cache</span><span class="sxs-lookup"><span data-stu-id="92541-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="92541-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="92541-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="92541-110">%USERPROFILE%\AppData\Lokal\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="92541-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="92541-111">Åbn SharePoint Designer 2013, og angiv kontoen igen for at se, om den virker.</span><span class="sxs-lookup"><span data-stu-id="92541-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="92541-112">Trin 3: [Aktiver moderne godkendelse til Office 2013 på Windows-enheder](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="92541-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>

<span data-ttu-id="92541-113">Trin 4: Administratorer skal **tillade brugerdefineret script** i Indstillingerne for SharePoint Administration for at tillade SharePoint Designer-forbindelsen.</span><span class="sxs-lookup"><span data-stu-id="92541-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="92541-114">Se [Tillad eller forhindre brugerdefineret script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="92541-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


