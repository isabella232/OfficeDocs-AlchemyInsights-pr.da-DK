---
title: Kalenderikonet vises ikke i Microsoft teams-klienten
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: e28b1c8d5d0feef1a743c8527db424af4c205fe9
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583344"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a><span data-ttu-id="768ad-102">Kalenderikonet vises ikke i Microsoft teams-klienten</span><span class="sxs-lookup"><span data-stu-id="768ad-102">Calendar icon isn't showing in Microsoft Teams client</span></span>

<span data-ttu-id="768ad-103">Fanen **kalender** i teams kræver adgang til en Exchange-postkasse via Exchange-Webtjenester.</span><span class="sxs-lookup"><span data-stu-id="768ad-103">The **Calendar** Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="768ad-104">Exchange-postkassen kan være online eller lokalt.</span><span class="sxs-lookup"><span data-stu-id="768ad-104">The Exchange mailbox can be Online, or On-Premises.</span></span> <span data-ttu-id="768ad-105">For online brugere, der ikke kan se fanen **kalender** , skal du kontrollere, at de [er givet i licens til en Exchange Online-postkasse, og at postkassen er aktiveret](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="768ad-105">For Online users who do not see the **Calendar** Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span> <span data-ttu-id="768ad-106">Hvis dine brugere har hjem lokalt, skal du bekræfte, at din hybrid konfiguration er i orden.</span><span class="sxs-lookup"><span data-stu-id="768ad-106">If your users are homed On-Premises, you need to confirm that your Hybrid configuration is healthy.</span></span> <span data-ttu-id="768ad-107">Brug [Guiden Hybridkonfiguration](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) til fejlfinding.</span><span class="sxs-lookup"><span data-stu-id="768ad-107">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span> <span data-ttu-id="768ad-108">Bemærk, at [Teams kræver Exchange 2016 CU3 eller højere](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="768ad-108">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>

<span data-ttu-id="768ad-109">Du kan finde flere oplysninger og fejlfindingstrin under [fejlfinding af problemer med Microsoft teams og Exchange Server-samspil](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).</span><span class="sxs-lookup"><span data-stu-id="768ad-109">For more information and troubleshooting steps, see [Troubleshoot Microsoft Teams and Exchange Server interaction issues](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).</span></span>
