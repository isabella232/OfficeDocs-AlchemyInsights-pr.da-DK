---
title: Kalenderikonet vises ikke i Teams-klient
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
- "9001219"
- "4375"
ms.openlocfilehash: f30cd5bda62756cf6b912ed150b4e59e7ca4d85d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684692"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="a6408-102">Kalenderikonet vises ikke i Teams-klient</span><span class="sxs-lookup"><span data-stu-id="a6408-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="a6408-103">Fanen Kalender i Teams kræver adgang til en Exchange-postkasse via Exchange Webtjenester.</span><span class="sxs-lookup"><span data-stu-id="a6408-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="a6408-104">Exchange-postkassen kan være online eller lokal.</span><span class="sxs-lookup"><span data-stu-id="a6408-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="a6408-105">Onlinebrugere, der ikke kan se fanen Kalender, skal sørge for, at de [har licens til en Exchange Online-postkasse, og at postkassen er aktiveret](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="a6408-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="a6408-106">Hvis brugeren har en gyldig postkasse i Exchange Online, men stadig ikke kan se fanen Kalender, er der måske problemer med netværket.</span><span class="sxs-lookup"><span data-stu-id="a6408-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="a6408-107">Brug [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/), og kør **forbindelsestesten for Microsoft Exchange-webtjenester** for den berørte bruger.</span><span class="sxs-lookup"><span data-stu-id="a6408-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="a6408-108">Læs til sidst [Teams-apps – politikker om konfiguration af apps](https://admin.teams.microsoft.com/policies/app-setup) for at sikre, at appen Kalender ikke er fjernet fra den politik, der gælder for brugeren (sandsynligvis **Global (standard for hele organisation standard)**.</span><span class="sxs-lookup"><span data-stu-id="a6408-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="a6408-109">Hvis dine brugere arbejder lokalt, skal du bekræfte, at din hybridkonfiguration er i orden.</span><span class="sxs-lookup"><span data-stu-id="a6408-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="a6408-110">Brug [Guiden Hybridkonfiguration](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) til fejlfinding.</span><span class="sxs-lookup"><span data-stu-id="a6408-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="a6408-111">Bemærk, at [Teams kræver Exchange 2016 CU3 eller højere](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="a6408-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
