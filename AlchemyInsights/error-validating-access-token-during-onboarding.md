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
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813682"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="79c3b-102">Fejlen "Der opstod en fejl under validering af adgangstoken" under onboarding af skrivebordsanalyse</span><span class="sxs-lookup"><span data-stu-id="79c3b-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="79c3b-103">Denne fejl observeres normalt, når godkendelsestokenet udløber.</span><span class="sxs-lookup"><span data-stu-id="79c3b-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="79c3b-104">Opdatering af siden opdaterer som regel tokenet.</span><span class="sxs-lookup"><span data-stu-id="79c3b-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="79c3b-105">Dette problem kan dog bevares, hvis der er anvendt nogen politikker for Betinget adgang på den konto, der bruges til on-board Desktop Analytics.</span><span class="sxs-lookup"><span data-stu-id="79c3b-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="79c3b-106">Du kan gennemse logonlogfilerne til Azure AD i Azure-portalen for at se, om der er nogen logonfejl for den konto, der bruges til onboarding af desktop analytics.</span><span class="sxs-lookup"><span data-stu-id="79c3b-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="79c3b-107">Hvis du vil have mere at vide om Betinget adgang, skal [du gå til Planlæg din installation af Betinget adgang.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)</span><span class="sxs-lookup"><span data-stu-id="79c3b-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>