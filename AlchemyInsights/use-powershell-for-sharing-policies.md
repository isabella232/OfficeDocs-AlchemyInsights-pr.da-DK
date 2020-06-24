---
title: Bruge PowerShell til delingspolitikker og organisationsrelationer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 717cdd6827e243ac6bf375209a911937c97088d2
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862054"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="b129f-102">Bruge PowerShell til delingspolitikker og organisationsrelationer</span><span class="sxs-lookup"><span data-stu-id="b129f-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="b129f-103">For organisationsrelationer skal du gennemgå de detaljerede syntaks- og parameteroplysninger for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) AND [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span><span class="sxs-lookup"><span data-stu-id="b129f-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="b129f-104">Hvis du vil oprette delingspolitik, skal du bruge [Ny delingspolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="b129f-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="b129f-105">Hvis du vil [anvende en delingspolitik på en postkasse eller bruger,](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) skal du bruge en kombination af [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) og [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) med den nyoprettede politik.</span><span class="sxs-lookup"><span data-stu-id="b129f-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="b129f-106">Hvis du vil [ændre, deaktivere eller fjerne en delingspolitik,](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) skal du bruge [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) og [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="b129f-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="b129f-107">**For fuld forståelse af dette emne kan du læse:**</span><span class="sxs-lookup"><span data-stu-id="b129f-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="b129f-108">Deling i Exchange Online</span><span class="sxs-lookup"><span data-stu-id="b129f-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)