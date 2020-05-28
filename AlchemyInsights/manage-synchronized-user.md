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
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Der kan ikke angives primær mailadresse, ændre brugerattributter eller fjerne/slette en synkroniseret bruger

Hvis katalogsynkronisering er aktiveret for dit miljø, kan nogle bruger- eller objektattributter ikke ændres ved hjælp af Microsoft 365 Administration.

Hvis du vil administrere synkroniserede brugere og alle deres attributter fuldt ud, skal du bruge dine lokale active directory-brugere og gruppeadministrationskonsol (adsiedit.msc).  

Du kan også ændre individuelle brugere eller attributter for synkroniserede brugere ved hjælp af powershell, f.eks. 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
