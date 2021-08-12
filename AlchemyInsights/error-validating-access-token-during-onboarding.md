---
title: Der opstod en fejl under validering af adgangstokenfejl under on-boarding af Desktop Analytics
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 1d6b840e731eaff537d8f74f9ce0af29af13bd390e701fb2835e8718b4521158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946609"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Fejlen "Der opstod en fejl under validering af adgangstoken" under onboarding af skrivebordsanalyse

Denne fejl observeres normalt, når godkendelsestokenet udløber. Opdatering af siden opdaterer som regel tokenet. Dette problem kan dog bevares, hvis der er anvendt nogen politikker for Betinget adgang på den konto, der bruges til on-board Desktop Analytics. Du kan gennemse logonlogfilerne til Azure AD i Azure-portalen for at se, om der er nogen logonfejl for den konto, der bruges til onboarding af desktop analytics.

Hvis du vil have mere at vide om Betinget adgang, skal [du gå til Planlæg din installation af Betinget adgang.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)