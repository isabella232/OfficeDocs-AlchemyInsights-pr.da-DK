---
title: SharePoint Online tilladelsesniveauer
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760687"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="0c4d2-102">SharePoint Designer forbindelsesproblemer</span><span class="sxs-lookup"><span data-stu-id="0c4d2-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="0c4d2-103">Hvis SharePoint Designer problemer med forbindelsen til SharePoint-websteder, skal du forsøge følgende fælles løsninger.</span><span class="sxs-lookup"><span data-stu-id="0c4d2-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please attempt the following common solutions.</span></span>

<span data-ttu-id="0c4d2-104">Trin 1: Kontroller, at SharePoint Designer er opdateret.</span><span class="sxs-lookup"><span data-stu-id="0c4d2-104">Step 1: Verify SharePoint Designer is updated.</span></span>

- [<span data-ttu-id="0c4d2-105">SharePoint Designer 2013</span><span class="sxs-lookup"><span data-stu-id="0c4d2-105">SharePoint Designer 2013</span></span>](https://www.microsoft.com/download/details.aspx?id=35491)

- [<span data-ttu-id="0c4d2-106">SharePoint Designer Service Pack 1 (SP1)</span><span class="sxs-lookup"><span data-stu-id="0c4d2-106">SharePoint Designer Service Pack 1 (SP1)</span></span>](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [<span data-ttu-id="0c4d2-107">Opdatering til SharePoint Designer 2013 (KB3114721)</span><span class="sxs-lookup"><span data-stu-id="0c4d2-107">Update for SharePoint Designer 2013 (KB3114721)</span></span>](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

<span data-ttu-id="0c4d2-108">Trin 2: Fjern de lokale cache-filer</span><span class="sxs-lookup"><span data-stu-id="0c4d2-108">Step 2: Clear the local cache files</span></span>

- <span data-ttu-id="0c4d2-109">Lukke SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="0c4d2-109">Close SharePoint Designer 2013.</span></span>

- <span data-ttu-id="0c4d2-110">Gå til følgende mapper til at fjerne cachelagrede filer på den lokale computer.</span><span class="sxs-lookup"><span data-stu-id="0c4d2-110">On the local computer, browse to the following folders to remove cached files.</span></span>

- <span data-ttu-id="0c4d2-111">Klik på Start, Kør og slette alle filer, der er fundet under hver af de nedenstående placeringer.</span><span class="sxs-lookup"><span data-stu-id="0c4d2-111">Click Start, Run and delete all files found under each of the below locations.</span></span>

<span data-ttu-id="0c4d2-112">%APPDATA%\Microsoft\Web server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="0c4d2-112">%APPDATA%\Microsoft\Web Server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

<span data-ttu-id="0c4d2-113">Åbn SharePoint Designer 2013 og angive kontoen igen for at se, hvis det virker.</span><span class="sxs-lookup"><span data-stu-id="0c4d2-113">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="0c4d2-114">Trin 3: [Aktivér moderne godkendelse for 2013 til Office på Windows-enheder](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="0c4d2-114">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span></span>

<span data-ttu-id="0c4d2-115">Trin 4: Administratorer skal tillade brugerdefineret Script til at tillade forbindelse til SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="0c4d2-115">Step 4: Administrators will need to Allow Custom Script to allow the SharePoint Designer connection.</span></span>

<span data-ttu-id="0c4d2-116">Se flere detaljerede oplysninger, eksempler og overvejelser i forbindelse med [Tillad eller forhindre brugerdefineret script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="0c4d2-116">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


