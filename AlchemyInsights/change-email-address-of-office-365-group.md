---
title: Skift mailadresse for en Microsoft 365-gruppe
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 8eaafae8650a8072cdfbec281afe6d5e93fea655
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819038"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="2913e-102">Skift mailadresse for en Microsoft 365-gruppe</span><span class="sxs-lookup"><span data-stu-id="2913e-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="2913e-103">Du kan ændre mailadressen på en Microsoft 365-gruppe ved hjælp af Administration.</span><span class="sxs-lookup"><span data-stu-id="2913e-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="2913e-104">Markér blot gruppen, og vælg @rediger mailadresse.</span><span class="sxs-lookup"><span data-stu-id="2913e-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="2913e-105">Du kan også bruge følgende EXO PowerShell-kommando til at ændre den primære SMTP-adresse for en Microsoft 365-gruppe:</span><span class="sxs-lookup"><span data-stu-id="2913e-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="2913e-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="2913e-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="2913e-107">Eksempel:</span><span class="sxs-lookup"><span data-stu-id="2913e-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
