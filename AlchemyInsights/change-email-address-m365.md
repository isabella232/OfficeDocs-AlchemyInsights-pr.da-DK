---
title: Skift mailadressen for en Microsoft 365-gruppe eller Microsoft Teams
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
ms.openlocfilehash: 7800a447c5dfcc8397121e1149921916ff7944ac
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819074"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a><span data-ttu-id="8e816-102">Skift mailadressen for en Microsoft 365-gruppe eller Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="8e816-102">Change email address of a Microsoft 365 group or Microsoft Teams</span></span>

<span data-ttu-id="8e816-103">Du kan ændre mailadressen for en Microsoft 365-gruppe eller Microsoft Teams ved at bruge [Microsoft 365 Administration](https://admin.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="8e816-103">You can change the email address of a Microsoft 365 group or Microsoft Teams by using the [Microsoft 365 admin center](https://admin.microsoft.com/).</span></span> <span data-ttu-id="8e816-104">Markér blot gruppen, og vælg @rediger mailadresse.</span><span class="sxs-lookup"><span data-stu-id="8e816-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="8e816-105">Du kan også bruge følgende EXO PowerShell-kommando til at ændre den primære SMTP-adresse for en Microsoft 365-gruppe/Teams:</span><span class="sxs-lookup"><span data-stu-id="8e816-105">You can also use the following EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group/Teams:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="8e816-106">Eksempel:</span><span class="sxs-lookup"><span data-stu-id="8e816-106">Example:</span></span>

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
