---
title: Adressering af Teams-logonfejl AADSTS9000411
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821981"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="fedc8-102">Adressering af Teams-logonfejl AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="fedc8-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="fedc8-103">Når du logger på Microsoft Teams, modtager du muligvis fejlen: Vi beklager, men vi har problemer med at logge dig på **AADSTS9000411: Anmodningen er ikke formateret korrekt. Parameteren "login_hint" duplikeres.**</span><span class="sxs-lookup"><span data-stu-id="fedc8-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="fedc8-104">For at løse dette problem skal du sørge for, at dine Microsoft Teams-klienter opdateres.</span><span class="sxs-lookup"><span data-stu-id="fedc8-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="fedc8-105">Du kan finde flere oplysninger om opdatering af din klient i [Opdater Microsoft Teams.](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)</span><span class="sxs-lookup"><span data-stu-id="fedc8-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="fedc8-106">Hvis du af en eller anden grund ikke kan opdatere din klient, rydder du de fleste cachelagrede data ved at logge af klienten.</span><span class="sxs-lookup"><span data-stu-id="fedc8-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="fedc8-107">Men hvis du stadig har problemer efter logoff/logon, skal du afslutte Teams og rydde din klientcache ved at gøre følgende:</span><span class="sxs-lookup"><span data-stu-id="fedc8-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="fedc8-108">Luk Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="fedc8-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="fedc8-109">Gå til: %appdata%\microsoft\teams, og slet alle filerne.</span><span class="sxs-lookup"><span data-stu-id="fedc8-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="fedc8-110">Genåå Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="fedc8-110">Reopen Microsoft Teams.</span></span>
