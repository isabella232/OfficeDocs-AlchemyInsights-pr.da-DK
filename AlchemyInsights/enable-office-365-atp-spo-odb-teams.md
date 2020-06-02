---
title: Aktivere Office 365 ATP til SharePoint, OneDrive og Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506912"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="85478-102">Aktivere avanceret beskyttelse mod office 365 til SharePoint Online, OneDrive og Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="85478-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="85478-103">Gå til https://protection.office.com og log på.</span><span class="sxs-lookup"><span data-stu-id="85478-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="85478-104">Vælg **Advarsler**  >  **Policy**  >  **om beskyttelsesstÃ evner til**politik for politik .</span><span class="sxs-lookup"><span data-stu-id="85478-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="85478-105">Vælg **Slå ATP til for SharePoint, OneDrive og Microsoft Teams**, og klik derefter på **Gem**.</span><span class="sxs-lookup"><span data-stu-id="85478-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="85478-106">(Anbefales) Kør [cmdlet'en Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) med parameteren **DisallowInfectedFileDownload** , der er angivet til *true,* som global administrator eller SharePoint Online-administrator.</span><span class="sxs-lookup"><span data-stu-id="85478-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="85478-107">(Anbefales) [Konfigurer beskeder](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for fundne filer.</span><span class="sxs-lookup"><span data-stu-id="85478-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="85478-108">ATP scanner nto-scanning af hver enkelt fil i SharePoint Online, OneDrive eller Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="85478-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="85478-109">Filer scannes asynkront gennem en proces, der bruger delings- og gæsteaktivitetshændelser sammen med smarte heuristik og trusselssignaler til at identificere skadelige filer.</span><span class="sxs-lookup"><span data-stu-id="85478-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="85478-110">Se [ATP for SharePoint, OneDrive og Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="85478-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>