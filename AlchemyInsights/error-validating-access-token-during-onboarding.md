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
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="e2983-102">Fejlen "der opstod en fejl under validering af adgangstoken" under skrivebordsanalyse Onboarding</span><span class="sxs-lookup"><span data-stu-id="e2983-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="e2983-103">Denne fejl er normalt observeret, når godkendelsestoken udløber.</span><span class="sxs-lookup"><span data-stu-id="e2983-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="e2983-104">Normalt opdaterer siden opdateringen af tokenet.</span><span class="sxs-lookup"><span data-stu-id="e2983-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="e2983-105">Dette problem kan dog vare ved, hvis der anvendes politikker for betinget adgang til den konto, der bruges til at foretage en skrivebordsanalyse om bord.</span><span class="sxs-lookup"><span data-stu-id="e2983-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="e2983-106">Du kan gennemse Azure AD-logonloggen på Azure-portalen for at se, om der er nogen Logonfejl for den konto, der bruges til desktop Analytics-Onboarding.</span><span class="sxs-lookup"><span data-stu-id="e2983-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="e2983-107">Du finder flere oplysninger om betinget adgang ved at besøge [Planlæg installationen af betinget adgang](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="e2983-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>