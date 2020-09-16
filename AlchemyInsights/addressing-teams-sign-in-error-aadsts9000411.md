---
title: AADSTS9000411 for teams-logon fejl
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
- "9000744"
- "5689"
ms.openlocfilehash: 8ca3793b8cd12b7ad2510ca0b3be58c32a61c14c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47687032"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="0038f-102">AADSTS9000411 for teams-logon fejl</span><span class="sxs-lookup"><span data-stu-id="0038f-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="0038f-103">Når du logger på Microsoft teams, får du muligvis fejlen: **vi beklager, men vi har problemer med at logge på AADSTS9000411: anmodningen er ikke formateret korrekt. Parameteren "login_hint" er duplikeret.**</span><span class="sxs-lookup"><span data-stu-id="0038f-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="0038f-104">For at løse dette problem skal du kontrollere, at dine Microsoft teams-klienter er opdateret.</span><span class="sxs-lookup"><span data-stu-id="0038f-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="0038f-105">Du kan finde flere oplysninger om opdatering af din klient i [opdatere Microsoft teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="0038f-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="0038f-106">Hvis du ikke kan opdatere din klient af en eller anden grund, kan du logge af klienten for at rydde de fleste cachelagrede data.</span><span class="sxs-lookup"><span data-stu-id="0038f-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="0038f-107">Men hvis du stadig har problemer efter logoff/logon, skal du afslutte teams og rydde din klientcache ved at gøre følgende:</span><span class="sxs-lookup"><span data-stu-id="0038f-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="0038f-108">Luk Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="0038f-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="0038f-109">Gå til:%AppData%\microsoft\teams og slet alle filerne.</span><span class="sxs-lookup"><span data-stu-id="0038f-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="0038f-110">Åbn Microsoft teams igen.</span><span class="sxs-lookup"><span data-stu-id="0038f-110">Reopen Microsoft Teams.</span></span>
