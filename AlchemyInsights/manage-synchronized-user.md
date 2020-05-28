---
title: Administrer synkroniseret bruger
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 84e337a7224fdd3c3ab7ad0f61240692fe007d5a
ms.sourcegitcommit: 82af227ac6d075e748e27c4ce6bdcf56628559cb
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/28/2020
ms.locfileid: "44407344"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="b2c8b-102">Der kan ikke angives primær mailadresse, ændre brugerattributter eller fjerne/slette en synkroniseret bruger</span><span class="sxs-lookup"><span data-stu-id="b2c8b-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="b2c8b-103">Hvis katalogsynkronisering er aktiveret for dit miljø, kan nogle bruger- eller objektattributter ikke ændres ved hjælp af Microsoft 365 Administration.</span><span class="sxs-lookup"><span data-stu-id="b2c8b-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="b2c8b-104">Hvis du vil administrere synkroniserede brugere og alle deres attributter fuldt ud, skal du bruge dine lokale active directory-brugere og gruppeadministrationskonsol (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="b2c8b-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="b2c8b-105">Du kan også ændre individuelle brugere eller attributter for synkroniserede brugere ved hjælp af powershell, f.eks.</span><span class="sxs-lookup"><span data-stu-id="b2c8b-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
