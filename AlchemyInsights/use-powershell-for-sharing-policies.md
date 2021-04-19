---
title: Bruge PowerShell til delingspolitikker og organisationsrelationer
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 9c52b876160f9577e6cefe7644c29d6fdf3b23fd
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826049"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>Bruge PowerShell til delingspolitikker og organisationsrelationer


For organisationsrelationer bedes du gennemgå de detaljerede syntaks- og parameteroplysninger for: [Hent SammensluttedeOplysninger](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [Ny-Organisationsrelation](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Angiv-Organisationsrelation](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  OG  [Fjern-Organisationsrelation](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Hvis du vil oprette en delingspolitik, skal du bruge [Ny-Delingspolitik](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). Hvis du vil  [anvende en delingspolitik på en postkasse eller bruger](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes),  skal du bruge en kombination  [Angiv-Postkasse](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) og [Hent-Postkasse](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) med den nyoprettede politik. Hvis du vil  [redigere, deaktivere eller fjerne en delingspolitik](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy),  skal du bruge  [Angiv-Delingspolitik](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) og [Fjern-Delingspolitik](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**For at få fuld forståelse for dette emne skal du læse:**

[Deling i Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)