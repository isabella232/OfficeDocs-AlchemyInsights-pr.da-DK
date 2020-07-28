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
# <a name="unable-to-change-username"></a><span data-ttu-id="5cd88-102">Brugernavnet kan ikke ændres</span><span class="sxs-lookup"><span data-stu-id="5cd88-102">Unable to change UserName</span></span>

<span data-ttu-id="5cd88-103">I nogle tilfælde overføres UPN-ændringer (UserPrincipalName) ikke til skyen.</span><span class="sxs-lookup"><span data-stu-id="5cd88-103">In some cases, UPN (UserPrincipalName) changes aren't propagated to the cloud.</span></span> <span data-ttu-id="5cd88-104">Du modtager muligvis valideringsfejl på Office 365-portalen eller kan ikke ændre brugernavnet eller mailadressen.</span><span class="sxs-lookup"><span data-stu-id="5cd88-104">You might receive validation errors in the Office 365 portal or be unable to change the username or email address.</span></span> <span data-ttu-id="5cd88-105">Du kan lÃ ̧se problemet ved manuelt at angive UserPrincipalName ved hjælp af denne PowerShell-kommando.</span><span class="sxs-lookup"><span data-stu-id="5cd88-105">To resolve this issue, manually set UserPrincipalName using this PowerShell command.</span></span>

<span data-ttu-id="5cd88-106">**Eksempel: Omdøbe en bruger**</span><span class="sxs-lookup"><span data-stu-id="5cd88-106">**Example: Rename a user**</span></span>

<span data-ttu-id="5cd88-107">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="5cd88-107">PowerShellCopy</span></span>

<span data-ttu-id="5cd88-108">PS C: \> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span><span class="sxs-lookup"><span data-stu-id="5cd88-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span></span>

<span data-ttu-id="5cd88-109">Denne kommando omdøber davidc@contoso.com til davidchew@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="5cd88-109">This command renames davidc@contoso.com to davidchew@contoso.com.</span></span>

<span data-ttu-id="5cd88-110">Yderligere oplysninger finder du i [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span><span class="sxs-lookup"><span data-stu-id="5cd88-110">For more information, see [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span></span>