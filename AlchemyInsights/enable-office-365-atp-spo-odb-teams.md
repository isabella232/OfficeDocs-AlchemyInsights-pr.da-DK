---
title: Aktivere Office 365 DTT for SharePoint, OneDrive og Microsoft-Team
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 601aec31e6556286fe5e0fd62827a037cbb6fe17
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/02/2019
ms.locfileid: "31030926"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="028aa-102">Aktivere Office 365 avancerede Threat Protection til SharePoint Online, OneDrive og Microsoft-Team</span><span class="sxs-lookup"><span data-stu-id="028aa-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="028aa-103">Gå til https://protection.office.com og logge på.</span><span class="sxs-lookup"><span data-stu-id="028aa-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="028aa-104">Vælg **trussel management** > **politik** > **Sikre vedhæftede filer**.</span><span class="sxs-lookup"><span data-stu-id="028aa-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="028aa-105">Vælg **Slå DTT for SharePoint, OneDrive, og Microsoft-Team**, og klik derefter på **Gem**.</span><span class="sxs-lookup"><span data-stu-id="028aa-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="028aa-106">(Anbefales) Som en global administrator eller en SharePoint Online-administratoren, køre [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) -cmdlet med parameteren **DisallowInfectedFileDownload** er indstillet til *Sand*.</span><span class="sxs-lookup"><span data-stu-id="028aa-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="028aa-107">(Anbefales) [Konfigurer påmindelser](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for fundne filer.</span><span class="sxs-lookup"><span data-stu-id="028aa-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="028aa-108">ATP vil nDu kan kun scanning hver enkelt fil i SharePoint Online, OneDrive eller Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="028aa-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="028aa-109">Filer scannes asynkront, gennem en proces, der bruger Deling og gæster aktivitet hændelser, sammen med intelligent heuristik og trussel signaler til at identificere skadelige filer.</span><span class="sxs-lookup"><span data-stu-id="028aa-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="028aa-110">Se [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="028aa-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>