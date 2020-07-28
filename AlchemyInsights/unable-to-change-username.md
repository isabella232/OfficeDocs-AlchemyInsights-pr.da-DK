---
title: Brugernavnet kan ikke ændres
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439101"
---
# <a name="unable-to-change-username"></a>Brugernavnet kan ikke ændres

I nogle tilfælde overføres UPN-ændringer (UserPrincipalName) ikke til skyen. Du modtager muligvis valideringsfejl på Office 365-portalen eller kan ikke ændre brugernavnet eller mailadressen. Du kan lÃ ̧se problemet ved manuelt at angive UserPrincipalName ved hjælp af denne PowerShell-kommando.

**Eksempel: Omdøbe en bruger**

PowerShellCopy

PS C: \> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"

Denne kommando omdøber davidc@contoso.com til davidchew@contoso.com.

Yderligere oplysninger finder du i [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).