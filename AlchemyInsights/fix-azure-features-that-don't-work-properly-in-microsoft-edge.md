---
title: Hvad du skal gøre, hvis Azure-funktionerne ikke fungerer korrekt i Microsoft Edge
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583309"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a><span data-ttu-id="4c0fd-102">Hvad du skal gøre, hvis Azure-funktionerne ikke fungerer korrekt i Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="4c0fd-102">What to do if Azure features don't work properly in Microsoft Edge</span></span>

<span data-ttu-id="4c0fd-103">Microsoft Edge har [kendte problemer](https://go.microsoft.com/fwlink/?linkid=2140608) , der er relateret til sikkerhedszoner og kan påvirke, hvordan Azure-brugere logger på Windows administration.</span><span class="sxs-lookup"><span data-stu-id="4c0fd-103">Microsoft Edge has [known issues](https://go.microsoft.com/fwlink/?linkid=2140608) that are related to security zones and might affect how Azure users log in to Windows Admin Center.</span></span> <span data-ttu-id="4c0fd-104">Hvis du har problemer med at bruge Azure-funktioner med Microsoft Edge, kan du prøve følgende trin:</span><span class="sxs-lookup"><span data-stu-id="4c0fd-104">If you're having trouble using Azure features with Microsoft Edge, try the following steps:</span></span>

1. <span data-ttu-id="4c0fd-105">I menuen **Start** skal du søge efter **Internet indstillinger** og vælge den.</span><span class="sxs-lookup"><span data-stu-id="4c0fd-105">In the **Start** menu, search for **Internet Options** and select it.</span></span>
2. <span data-ttu-id="4c0fd-106">Gå til fanen **sikkerhed** i dialogboksen **Egenskaber for internettet** .</span><span class="sxs-lookup"><span data-stu-id="4c0fd-106">In the **Internet Properties** dialog box, go to the **Security** tab.</span></span>
3. <span data-ttu-id="4c0fd-107">Vælg zonen **websteder, du har tillid** til, og vælg derefter knappen **websteder** .</span><span class="sxs-lookup"><span data-stu-id="4c0fd-107">Select the **Trusted sites** zone and then select the **Sites** button.</span></span>
4. <span data-ttu-id="4c0fd-108">I dialogboksen websteder, du **har tillid til** , skal du tilføje din gateway-URL samt [https://login.microsoftonline.com](https://login.microsoftonline.com) og [https://login.live.com](https://login.live.com) derefter vælge **Luk**.</span><span class="sxs-lookup"><span data-stu-id="4c0fd-108">In the **Trusted sites** dialog box, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
5. <span data-ttu-id="4c0fd-109">Gå til fanen **beskyttelse af personlige oplysninger** i dialogboksen **Egenskaber for internettet** .</span><span class="sxs-lookup"><span data-stu-id="4c0fd-109">In the **Internet Properties** dialog box, go to the **Privacy** tab.</span></span>
6. <span data-ttu-id="4c0fd-110">Vælg **Indstillinger** i sektionen **blokering af pop op-vinduer** .</span><span class="sxs-lookup"><span data-stu-id="4c0fd-110">In the **Pop-up Blocker** section, select **Settings**.</span></span> <span data-ttu-id="4c0fd-111">I den dialogboks, der åbnes, skal du tilføje din gateway-URL samt [https://login.microsoftonline.com](https://login.microsoftonline.com) og [https://login.live.com](https://login.live.com) derefter vælge **Luk**.</span><span class="sxs-lookup"><span data-stu-id="4c0fd-111">In the dialog box that opens, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
