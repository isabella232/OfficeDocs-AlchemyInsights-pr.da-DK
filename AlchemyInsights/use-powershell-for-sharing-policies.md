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
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>Bruge PowerShell til delingspolitikker og organisationsrelationer


For organisationsrelationer skal du gennemgå de detaljerede syntaks- og parameteroplysninger for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) AND [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Hvis du vil oprette delingspolitik, skal du bruge [Ny delingspolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). Hvis du vil [anvende en delingspolitik på en postkasse eller bruger,](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) skal du bruge en kombination af [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) og [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) med den nyoprettede politik. Hvis du vil [ændre, deaktivere eller fjerne en delingspolitik,](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) skal du bruge [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) og [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**For fuld forståelse af dette emne kan du læse:**

[Deling i Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)