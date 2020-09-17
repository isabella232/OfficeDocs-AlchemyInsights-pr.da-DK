---
title: Der opstod fejl under validering af fejl i adgangstoken under skrivebords analyse
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783545"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Fejlmeddelelsen "der opstod en fejl under validering af adgangstoken" under skrivebords analyse

Denne fejl observeres normalt, når godkendelses tokenet udløber. Hvis du opdaterer siden, opdateres tokenet normalt. Dette problem kan dog bevares, hvis der er anvendt politikker for betinget adgang på den konto, der bruges til skrivebords analyse på den indbyggede computer. Du kan gennemse logfilerne i Azure AD, når du er logget på Azure-portalen for at se, om der er problemer med logon på den konto, der bruges til Onboarding af skrivebords analyse.

Hvis du vil have mere at vide om betinget adgang, skal du se [plan lægge din installation af betinget adgang](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).