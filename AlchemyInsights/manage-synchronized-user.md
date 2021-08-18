---
title: Administrere synkroniseret bruger
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
- "9000609"
- "2444"
ms.openlocfilehash: bfa66492397adfd121fd3c9ddb2c190394cbc9a771a3e2c2db656ad438e404f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114766"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Det er ikke muligt at angive primær mailadresse, ændre brugerattributter eller fjerne/slette en synkroniseret bruger

Hvis katalogsynkronisering er aktiveret for dit miljø, kan nogle bruger- eller objektattributter ikke ændres ved hjælp Microsoft 365 Administration.

For at administrere synkroniserede brugere og alle deres attributter fuldt ud skal du bruge din lokale active directory-brugere og gruppeadministrationskonsol (adsiedit.msc).  

Alternativt kan du ændre individuelle brugere eller attributter for synkroniserede brugere ved hjælp af PowerShell, som vist i disse almindelige eksempler:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
