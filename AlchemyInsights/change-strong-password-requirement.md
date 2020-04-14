---
title: Skift krav om stærk adgangskode
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: 21f80a7cc8b00ac56acdb05add1e1bfdfac9d827
ms.sourcegitcommit: c061f1dfa6f557a9ec083dd030b73b121d9864ea
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/14/2020
ms.locfileid: "43286257"
---
# <a name="change-strong-password-requirement"></a>Ændre stort krav til adgangskode

Microsoft kræver som standard stærke adgangskoder. 

Ved hjælp af PowerShell kan du deaktivere stærke adgangskoder for bestemte brugere med denne kommando:<br>
*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired $false*

- [Flere oplysninger om adgangskodepolitik](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Sådan opretter du forbindelse til Office 365 med PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Flere oplysninger om PowerShell MsolUser-kommandoer](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
- [Angive, at en enkelt brugers adgangskode aldrig udløber](https://docs.microsoft.com/microsoft-365/admin/add-users/set-password-to-never-expire)
