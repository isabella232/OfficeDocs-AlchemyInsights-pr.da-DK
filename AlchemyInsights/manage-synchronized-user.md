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
ms.openlocfilehash: 5a383bdd17c5fa055c35a923ca36e0e0f6d429e4
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/28/2019
ms.locfileid: "35380499"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Kunne ikke indstille primær e-mail-adresse eller ændre brugerattributter

Hvis directory-synkronisering er aktiveret for miljøet vil nogle bruger- eller attributter kan ikke ændres ved hjælp af Admin Center.
For at administrere fuldt synkroniserede brugere og deres attributter, skal du bruge dit lokale active directory-brugere og -grupper administrationskonsollen (adsiedit.msc).  

Du kan også ændre individuelle brugere eller attributter for synkroniserede brugere ved hjælp af powershell, som vist i følgende almindelige eksempler: 
- Set-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Set-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "testbruger" - Efternavn "Bruger"-afsnit "Chef"-afdeling "T"
- Fjern-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com