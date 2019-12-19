---
title: Der opstod en fejl under validering af adgangstokenfejl under skrivebordsanalyse på boarding
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741148"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Fejlen "der opstod en fejl under validering af adgangstoken" under skrivebordsanalyse Onboarding

Denne fejl er normalt observeret, når godkendelsestoken udløber. Normalt opdaterer siden opdateringen af tokenet. Dette problem kan dog vare ved, hvis der anvendes politikker for betinget adgang til den konto, der bruges til at foretage en skrivebordsanalyse om bord. Du kan gennemse Azure AD-logonloggen på Azure-portalen for at se, om der er nogen Logonfejl for den konto, der bruges til desktop Analytics-Onboarding.

Du finder flere oplysninger om betinget adgang ved at besøge [Planlæg installationen af betinget adgang](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).