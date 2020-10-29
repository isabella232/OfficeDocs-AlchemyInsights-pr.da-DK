---
title: Aktivér Office 365 DTT til SharePoint, OneDrive og Microsoft teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: bef43656097c6f27677172899df1ada7900a9b64
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801041"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="3ae2d-102">Aktivér Microsoft Defender til Office 365 til SharePoint Online, OneDrive og Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="3ae2d-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="3ae2d-103">Gå til https://protection.office.com og log på.</span><span class="sxs-lookup"><span data-stu-id="3ae2d-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="3ae2d-104">Vælg politik for **trussels administrations**  >  **politik**  >  **sikre vedhæftede filer** .</span><span class="sxs-lookup"><span data-stu-id="3ae2d-104">Choose **Threat management** > **Policy** > **Safe Attachments** .</span></span>
3. <span data-ttu-id="3ae2d-105">Vælg **Aktivér DTT for SharePoint, OneDrive og Microsoft teams** , og klik derefter på **Gem** .</span><span class="sxs-lookup"><span data-stu-id="3ae2d-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams** , and then click **Save** .</span></span>
4. <span data-ttu-id="3ae2d-106">Anbefales Som global administrator eller SharePoint Online-administrator skal du køre cmdlet'en [set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) , hvor parameteren **DisallowInfectedFileDownload** er angivet til *sand* .</span><span class="sxs-lookup"><span data-stu-id="3ae2d-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true* .</span></span>
5. <span data-ttu-id="3ae2d-107">Anbefales [Konfigurere beskeder](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for registrerede filer.</span><span class="sxs-lookup"><span data-stu-id="3ae2d-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="3ae2d-108">DTT vil stræbe i at scanne hver enkelt fil i SharePoint Online, OneDrive eller Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="3ae2d-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="3ae2d-109">Filer scannes asynkront via en proces, der bruger aktiviteter til deling og gæst, samt smarte heuristik-og trussels signaler til at identificere ondsindede filer.</span><span class="sxs-lookup"><span data-stu-id="3ae2d-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="3ae2d-110">Se [DTT til SharePoint, OneDrive og Microsoft teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="3ae2d-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>