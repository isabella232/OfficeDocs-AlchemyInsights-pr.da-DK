---
title: Ændre mailadressen på en Microsoft 365-gruppe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/27/2020
ms.locfileid: "44282709"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a><span data-ttu-id="ea5d5-102">Ændre mailadressen på en Microsoft 365-gruppe</span><span class="sxs-lookup"><span data-stu-id="ea5d5-102">Change email address of an Microsoft 365 group</span></span>

<span data-ttu-id="ea5d5-103">Du kan ændre mailadressen på en Microsoft 365-gruppe ved hjælp af Administration.</span><span class="sxs-lookup"><span data-stu-id="ea5d5-103">You can change the email address of an Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="ea5d5-104">Du skal blot vælge gruppen og vælge @edit mailadresse.</span><span class="sxs-lookup"><span data-stu-id="ea5d5-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="ea5d5-105">Du kan også bruge at følge KOMMANDOEN EXO PowerShell til at ændre den primære SMTP-adresse for en Microsoft 365-gruppe:</span><span class="sxs-lookup"><span data-stu-id="ea5d5-105">You can also use following the EXO PowerShell command to change the primary SMTP address of an Microsoft 365 group:</span></span>

<span data-ttu-id="ea5d5-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="ea5d5-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="ea5d5-107">Eksempel:</span><span class="sxs-lookup"><span data-stu-id="ea5d5-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
