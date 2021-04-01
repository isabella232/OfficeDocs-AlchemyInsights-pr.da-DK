---
title: Angiv Microsoft Edge som standardbrowser på en macOS-enhed
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491424"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a><span data-ttu-id="95216-102">Angiv Microsoft Edge som standardbrowser på en macOS-enhed</span><span class="sxs-lookup"><span data-stu-id="95216-102">Set Microsoft Edge as the default browser on a macOS device</span></span>

<span data-ttu-id="95216-103">Brug en af disse to metoder til at angive Microsoft Edge som standardbrowser:</span><span class="sxs-lookup"><span data-stu-id="95216-103">Use one of these two methods to set Microsoft Edge as the default browser:</span></span>

<span data-ttu-id="95216-104">Metode 1: Flash enheden med et billede af macOS, hvor Microsoft Edge allerede er angivet som standardbrowser.</span><span class="sxs-lookup"><span data-stu-id="95216-104">Method 1: Flash the device with an image of macOS where Microsoft Edge has already been set as the default browser.</span></span>

<span data-ttu-id="95216-105">Metode 2: Angiv politikken DefaultBrowserSettingEnabled for at bede brugeren om at angive Microsoft Edge som standardbrowser.</span><span class="sxs-lookup"><span data-stu-id="95216-105">Method 2: Set the DefaultBrowserSettingEnabled policy to prompt the user to set Microsoft Edge as the default browser.</span></span>

<span data-ttu-id="95216-106">Begge metoder giver en bruger mulighed for at ændre standardbrowseren.</span><span class="sxs-lookup"><span data-stu-id="95216-106">Either method allows a user to change the default browser.</span></span> <span data-ttu-id="95216-107">Vi anbefaler derfor, at du installerer politikken DefaultBrowserSettingEnabled, også selvom du har brugt metode 1.</span><span class="sxs-lookup"><span data-stu-id="95216-107">For this reason, we recommend that you deploy the DefaultBrowserSettingEnabled policy even if you used method 1.</span></span> <span data-ttu-id="95216-108">Hvis en bruger ændrer standardbrowseren, efter politikken er implementeret, beder politikken brugeren om at indstille standardbrowseren tilbage til Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="95216-108">If a user changes the default browser after the policy is deployed, the policy prompts the user to set the default browser back to Microsoft Edge.</span></span>
