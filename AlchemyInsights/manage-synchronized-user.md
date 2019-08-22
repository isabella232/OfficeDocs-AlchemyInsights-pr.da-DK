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
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="fd0aa-102">Kunne ikke indstille primær e-mail-adresse eller ændre brugerattributter</span><span class="sxs-lookup"><span data-stu-id="fd0aa-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="fd0aa-103">Hvis directory-synkronisering er aktiveret for miljøet, vil nogle bruger- eller attributter kan ikke ændres ved hjælp af Microsoft 365 admin center.</span><span class="sxs-lookup"><span data-stu-id="fd0aa-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="fd0aa-104">For at administrere fuldt synkroniserede brugere og deres attributter, skal du bruge dit lokale active directory-brugere og -grupper administrationskonsollen (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="fd0aa-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="fd0aa-105">Du kan også ændre individuelle brugere eller attributter for synkroniserede brugere ved hjælp af powershell, som vist i følgende almindelige eksempler:</span><span class="sxs-lookup"><span data-stu-id="fd0aa-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="fd0aa-106">Set-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="fd0aa-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="fd0aa-107">Set-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "testbruger" - Efternavn "Bruger"-afsnit "Chef"-afdeling "T"</span><span class="sxs-lookup"><span data-stu-id="fd0aa-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="fd0aa-108">Fjern-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="fd0aa-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>