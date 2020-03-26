---
title: Kalenderikonet vises ikke i Teams-klient
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 21692639fb746b2e5aab3dfc8894293d5dc890ac
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931983"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="4b254-102">Kalenderikonet vises ikke i Teams-klient</span><span class="sxs-lookup"><span data-stu-id="4b254-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="4b254-103">Fanen Kalender i Teams kræver adgang til en Exchange-postkasse via Exchange Webtjenester.</span><span class="sxs-lookup"><span data-stu-id="4b254-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="4b254-104">Exchange-postkassen kan være online eller lokal.</span><span class="sxs-lookup"><span data-stu-id="4b254-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="4b254-105">Onlinebrugere, der ikke kan se fanen Kalender, skal sørge for, at de [har licens til en Exchange Online-postkasse, og at postkassen er aktiveret](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="4b254-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="4b254-106">Hvis brugeren har en gyldig postkasse i Exchange Online, men stadig ikke kan se fanen Kalender, er der måske problemer med netværket.</span><span class="sxs-lookup"><span data-stu-id="4b254-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="4b254-107">Brug [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/), og kør **forbindelsestesten for Microsoft Exchange-webtjenester** for den berørte bruger.</span><span class="sxs-lookup"><span data-stu-id="4b254-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="4b254-108">Læs til sidst [Teams-apps – politikker om konfiguration af apps](https://admin.teams.microsoft.com/policies/app-setup) for at sikre, at appen Kalender ikke er fjernet fra den politik, der gælder for brugeren (sandsynligvis **Global (standard for hele organisation standard)**.</span><span class="sxs-lookup"><span data-stu-id="4b254-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="4b254-109">Hvis dine brugere arbejder lokalt, skal du bekræfte, at din hybridkonfiguration er i orden.</span><span class="sxs-lookup"><span data-stu-id="4b254-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="4b254-110">Brug [Guiden Hybridkonfiguration](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) til fejlfinding.</span><span class="sxs-lookup"><span data-stu-id="4b254-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="4b254-111">Bemærk, at [Teams kræver Exchange 2016 CU3 eller højere](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="4b254-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
