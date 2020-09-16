---
title: Velkomstmeddelelse i Microsoft 365-grupper
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
- "5685"
ms.openlocfilehash: de16ca6021441bf6cb781106b7f3da8eed86b0f1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725833"
---
# <a name="welcome-message-in-microsoft-365-groups"></a>Velkomstmeddelelse i Microsoft 365-grupper

Nye brugere, der forbinder Microsoft 365-gruppe, får velkomstmail, hvis egenskaben "UnifiedGroupWelcomeMessageEnabled" er sand.

Hvis du vil deaktivere velkomstmeddelelsen, skal du bruge følgende [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) -kommando:

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
