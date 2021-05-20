---
title: Aktivér Office 365 ATP for SharePoint, OneDrive og Microsoft Teams
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
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543922"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="fdb3e-102">Aktivér Microsoft Defender Office 365 til SharePoint Online, OneDrive og Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="fdb3e-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="fdb3e-103">Gå til https://protection.office.com , og log på.</span><span class="sxs-lookup"><span data-stu-id="fdb3e-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="fdb3e-104">Vælg **Politik om sikkerhed i** forbindelse  >  **med** sikkerhed i forbindelse med sikkerhed i forbindelse med  >  **trusler**.</span><span class="sxs-lookup"><span data-stu-id="fdb3e-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="fdb3e-105">Vælg **Slå Defender til for Office 365 for SharePoint, OneDrive og Microsoft Teams**, og klik derefter på **Gem**.</span><span class="sxs-lookup"><span data-stu-id="fdb3e-105">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="fdb3e-106">(Anbefalet) Som global administrator eller SharePoint Online-administrator skal du køre [Set-SPOTenant-cmdlet'en](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) med parameteren **DisallowInfectedFileDownload** angivet til *sand*.</span><span class="sxs-lookup"><span data-stu-id="fdb3e-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="fdb3e-107">(Anbefalet) [Konfigurer beskeder for](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) registrerede filer.</span><span class="sxs-lookup"><span data-stu-id="fdb3e-107">(Recommended) [Set up alerts](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="fdb3e-108">Microsoft Defender for Office 365 scanner ikke hver enkelt fil i SharePoint Online, OneDrive eller Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="fdb3e-108">Microsoft Defender for Office 365 will not scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="fdb3e-109">Filer scannes asynkront gennem en proces, der bruger delings- og gæsteaktivitetshændelser sammen med smarte heuristiske og trusselssignaler til at identificere skadelige filer.</span><span class="sxs-lookup"><span data-stu-id="fdb3e-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="fdb3e-110">Se [Microsoft Defender for Office 365 for SharePoint, OneDrive og Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="fdb3e-110">See [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>