---
title: Skift mailadresse for en Microsoft 365-gruppe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: a2605bcd66f61de811ebb6e273e4ef1cff2b0119
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47733681"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="b073f-102">Skift mailadresse for en Microsoft 365-gruppe</span><span class="sxs-lookup"><span data-stu-id="b073f-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="b073f-103">Du kan ændre mailadressen til en Microsoft 365-gruppe ved hjælp af administrations centeret.</span><span class="sxs-lookup"><span data-stu-id="b073f-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="b073f-104">Du skal bare markere gruppen og vælge @edit mailadresse.</span><span class="sxs-lookup"><span data-stu-id="b073f-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="b073f-105">Du kan også bruge følgende EXO PowerShell-kommando til at ændre den primære SMTP-adresse for en Microsoft 365-gruppe:</span><span class="sxs-lookup"><span data-stu-id="b073f-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="b073f-106">Set-Unifiedgrouphttps <Group Name> -PrimarySmtpAddress <new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="b073f-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="b073f-107">:</span><span class="sxs-lookup"><span data-stu-id="b073f-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
