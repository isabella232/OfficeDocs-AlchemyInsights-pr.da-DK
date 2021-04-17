---
title: Skift krav til stærk adgangskode
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: cf5cab9a1c2dd4226997d93417dc7104347f8a6e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818462"
---
# <a name="change-strong-password-requirement"></a>Skift krav til stærk adgangskode

Microsoft kræver stærke adgangskoder som standard.

Ved hjælp af PowerShell kan du deaktivere stærke adgangskoder for bestemte brugere med disse kommandoer:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

Hvis du vil deaktivere stærke adgangskoder for alle brugere, skal du bruge:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [Flere oplysninger om adgangskodepolitik](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Sådan opretter du forbindelse til Microsoft 365 med PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Flere oplysninger om PowerShell MsolUser-kommandoer](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
