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
ms.openlocfilehash: 48df03b1397b0e924aa878cea3d1cac07ca862c3636c1273d10f4841a03fddcf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998460"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>Bruge PowerShell til delingspolitikker og organisationsrelationer


For organisationsrelationer bedes du gennemgå de detaljerede syntaks- og parameteroplysninger for: [Hent SammensluttedeOplysninger](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [Ny-Organisationsrelation](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Angiv-Organisationsrelation](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  OG  [Fjern-Organisationsrelation](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Hvis du vil oprette en delingspolitik, skal du bruge [Ny-Delingspolitik](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). Hvis du vil  [anvende en delingspolitik på en postkasse eller bruger](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes),  skal du bruge en kombination  [Angiv-Postkasse](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) og [Hent-Postkasse](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) med den nyoprettede politik. Hvis du vil  [redigere, deaktivere eller fjerne en delingspolitik](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy),  skal du bruge  [Angiv-Delingspolitik](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) og [Fjern-Delingspolitik](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**For at få fuld forståelse for dette emne skal du læse:**

[Deling i Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)