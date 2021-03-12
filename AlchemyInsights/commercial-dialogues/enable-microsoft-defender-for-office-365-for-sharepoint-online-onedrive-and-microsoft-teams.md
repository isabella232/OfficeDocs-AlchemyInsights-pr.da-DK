---
title: Aktivér Microsoft Defender til Office 365 til SharePoint Online, OneDrive og Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744115"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="6c4b8-102">Aktivér Microsoft Defender til Office 365 til SharePoint Online, OneDrive og Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="6c4b8-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive and Microsoft Teams</span></span>

1. <span data-ttu-id="6c4b8-103">Ved hjælp af din globale administrator eller sikkerhedsadministratorens legitimationsoplysninger skal du logge på [Office 365 Security and Compliance Center.](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="6c4b8-103">Using your global admin or security admin credentials, log in to the [Office 365 Security and Compliance Center](https://protection.office.com/).</span></span>
2. <span data-ttu-id="6c4b8-104">Vælg **Trusselsadministration** i venstre rude, og vælg derefter Vedhæftede   >  [filer, der er beskyttet med politik.](https://protection.office.com/safeattachment)</span><span class="sxs-lookup"><span data-stu-id="6c4b8-104">Select **Threat management** in the left pane, and then select **Policy** > [Safe attachments](https://protection.office.com/safeattachment).</span></span>
3. <span data-ttu-id="6c4b8-105">Vælg **Slå Microsoft Defender til for Office 365 til SharePoint, OneDrive** og Microsoft Teams, og vælg derefter **Gem.**</span><span class="sxs-lookup"><span data-stu-id="6c4b8-105">Select **Turn on Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then select **Save**.</span></span>
    > [!TIP]
    >
    > - <span data-ttu-id="6c4b8-106">Som global administrator eller SharePoint Online-administrator skal du køre følgende PowerShell-cmdlet med parameteren **DisallowInfectedFileDownload** angivet til *sand:* [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span><span class="sxs-lookup"><span data-stu-id="6c4b8-106">As a global admin or a SharePoint Online admin, run the following PowerShell cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span></span>
    > - [<span data-ttu-id="6c4b8-107">Konfigurere beskeder for registrerede filer</span><span class="sxs-lookup"><span data-stu-id="6c4b8-107">Set up alerts for detected files</span></span>](https://go.microsoft.com/fwlink/?linkid=2092110)

<span data-ttu-id="6c4b8-108">Du kan finde flere oplysninger [i Microsoft Defender til Office 365 til SharePoint, OneDrive og Microsoft Teams.](https://go.microsoft.com/fwlink/?linkid=2092041)</span><span class="sxs-lookup"><span data-stu-id="6c4b8-108">For more information, see [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).</span></span>
