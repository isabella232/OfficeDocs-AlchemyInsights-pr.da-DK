---
title: Administrere synkroniseret bruger
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
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36541979"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Kunne ikke indstille primær e-mail-adresse eller ændre brugerattributter

Hvis directory-synkronisering er aktiveret for miljøet, vil nogle bruger- eller attributter kan ikke ændres ved hjælp af Microsoft 365 admin center.

For at administrere fuldt synkroniserede brugere og deres attributter, skal du bruge dit lokale active directory-brugere og -grupper administrationskonsollen (adsiedit.msc).  

Du kan også ændre individuelle brugere eller attributter for synkroniserede brugere ved hjælp af powershell, som vist i følgende almindelige eksempler: 
- Set-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Set-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "testbruger" - Efternavn "Bruger"-afsnit "Chef"-afdeling "T"
- Fjern-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com