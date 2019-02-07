---
title: Angive eller ændre tilladelser til offentlige mapper
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 8/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: 8e6a51bcc47eac7e76f55700091ecd86bc1634d7
ms.sourcegitcommit: 5dee2fcb492bd922092a6de8045a95febe57b97e
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/06/2019
ms.locfileid: "29759814"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="77e3f-102">Tilladelser og offentlige mapper</span><span class="sxs-lookup"><span data-stu-id="77e3f-102">Permissions and Public Folders</span></span>

<span data-ttu-id="77e3f-103">Du kan ændre tilladelserne på dine offentlige mapper ved hjælp af Outlook, Exchange admin center (EAC) eller PowerShell:</span><span class="sxs-lookup"><span data-stu-id="77e3f-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="77e3f-104">Outlook-oplysninger, [skal du klikke her](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span><span class="sxs-lookup"><span data-stu-id="77e3f-104">For Outlook instructions, [click here](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="77e3f-p101">EAC, finde [denne artikel](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for at få instruktioner. Du kan klikke [her](https://support.office.com/article/ https://outlook.office365.com/ecp/.aspx) til at navigere til EAC.</span><span class="sxs-lookup"><span data-stu-id="77e3f-p101">For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions. You can click [here](https://support.office.com/article/ https://outlook.office365.com/ecp/.aspx) to navigate to EAC.</span></span> 
    
- <span data-ttu-id="77e3f-p102">Powershell, finde [denne artikel](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for at få vejledning i brugen af cmdlet accepterer Tilføj PublicFolderClientPermission. Hvis du har brug for vejledning til at oprette forbindelse til Exchange Powershell, skal du klikke [her](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span><span class="sxs-lookup"><span data-stu-id="77e3f-p102">For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet. If you need instructions to connect to Exchange Powershell, click [here](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="77e3f-p103">Hvis **eksterne brugere kan ikke sende e-mails til en offentlig mappe med e-mail-aktiveret**, årsagen kan være, at den offentlige mappe mangler tilladelser kræves for eksterne e-mail-levering. Du kan løse problemet ved hjælp af Outlook-vejledningen [her](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)eller PowerShell vejledningen [her](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span><span class="sxs-lookup"><span data-stu-id="77e3f-p103">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery. You can fix this using the Outlook instructions [here](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

