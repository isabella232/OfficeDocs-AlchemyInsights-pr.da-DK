---
title: Microsoft Edge-Brugeragentstreng (skrivebord)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003862"
- "6914"
ms.openlocfilehash: b4106dde1e09e0ce07b4b9adc2b2984cc5609c3b
ms.sourcegitcommit: 3c6e777d6679a24108171e9aa3f9379a8d44e001
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/09/2020
ms.locfileid: "49677378"
---
# <a name="microsoft-edge-user-agent-string-desktop"></a><span data-ttu-id="69441-102">Microsoft Edge-Brugeragentstreng (skrivebord)</span><span class="sxs-lookup"><span data-stu-id="69441-102">Microsoft Edge user agent string (Desktop)</span></span>

<span data-ttu-id="69441-103">Brugeragent-strenge (UA) kan bruges til at registrere, hvilken version af en bestemt browser der bruges på et bestemt operativsystem.</span><span class="sxs-lookup"><span data-stu-id="69441-103">User agent (UA) strings can be used to detect what version of a specific browser is being used on a certain operating system.</span></span> <span data-ttu-id="69441-104">Ligesom andre browsere indeholder Microsoft Edge disse oplysninger i HTTP-headeren "bruger agent", hver gang der foretages en anmodning til et websted.</span><span class="sxs-lookup"><span data-stu-id="69441-104">Like other browsers, Microsoft Edge includes this information in the "User-Agent" HTTP header whenever it makes a request to a site.</span></span> <span data-ttu-id="69441-105">Du kan også få adgang til browserens versionsoplysninger via JavaScript ved at forespørge værdien af "Navigator. userAgent".</span><span class="sxs-lookup"><span data-stu-id="69441-105">The browser-version information can also be accessed via JavaScript by querying the value of "navigator.userAgent".</span></span>

<span data-ttu-id="69441-106">Vi anbefaler, at webudvikler gør brug af funktionsregistrering, når det er muligt for at forbedre kodens opretholdelse, reducere kode fragility og eliminere risikoen for brud på kode i tilfælde af fremtidige UA-streng opdateringer.</span><span class="sxs-lookup"><span data-stu-id="69441-106">We recommend that web developers make use of feature detection whenever possible to improve code maintainability, reduce code fragility, and eliminate the risk of code breakage in the event of future UA string updates.</span></span>

<span data-ttu-id="69441-107">Du kan finde flere oplysninger i [Microsoft Edge user agent-streng (desktop)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span><span class="sxs-lookup"><span data-stu-id="69441-107">For more information, see [Microsoft Edge User Agent String (Desktop)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span></span>