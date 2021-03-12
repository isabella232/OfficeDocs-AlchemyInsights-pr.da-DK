---
title: Bruge PowerShell til delingspolitikker og organisationsrelationer
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
- "3800014"
- "898"
ms.openlocfilehash: cd1d34e4dae474e61c799ca9234b2f18c718f27b
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709460"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="f6dac-102">Bruge PowerShell til delingspolitikker og organisationsrelationer</span><span class="sxs-lookup"><span data-stu-id="f6dac-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="f6dac-103">For organisationsrelationer bedes du gennemgå de detaljerede syntaks- og parameteroplysninger for: [Hent SammensluttedeOplysninger](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [Ny-Organisationsrelation](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Angiv-Organisationsrelation](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  OG  [Fjern-Organisationsrelation](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span><span class="sxs-lookup"><span data-stu-id="f6dac-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="f6dac-104">Hvis du vil oprette en delingspolitik, skal du bruge [Ny-Delingspolitik](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="f6dac-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="f6dac-105">Hvis du vil  [anvende en delingspolitik på en postkasse eller bruger](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes),  skal du bruge en kombination  [Angiv-Postkasse](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) og [Hent-Postkasse](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) med den nyoprettede politik.</span><span class="sxs-lookup"><span data-stu-id="f6dac-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="f6dac-106">Hvis du vil  [redigere, deaktivere eller fjerne en delingspolitik](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy),  skal du bruge  [Angiv-Delingspolitik](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) og [Fjern-Delingspolitik](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="f6dac-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="f6dac-107">**For at få fuld forståelse for dette emne skal du læse:**</span><span class="sxs-lookup"><span data-stu-id="f6dac-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="f6dac-108">Deling i Exchange Online</span><span class="sxs-lookup"><span data-stu-id="f6dac-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)