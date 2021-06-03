---
title: Slutpunkt DLP ikke installeret på brugerens enhed
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/27/2021
ms.locfileid: "52731408"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a><span data-ttu-id="eed67-102">Slutpunkt DLP ikke installeret på brugerens enhed</span><span class="sxs-lookup"><span data-stu-id="eed67-102">Endpoint DLP not deployed to user's device</span></span>

<span data-ttu-id="eed67-103">Hvis indstillingen til forebyggelse af datatab på slutpunkter (DLP) ikke er anvendt på en brugers enhed, skal du bekræfte, at du opfylder følgende krav:</span><span class="sxs-lookup"><span data-stu-id="eed67-103">If the Endpoint data loss prevention (DLP) setting has not applied to a user's device, confirm you meet these requirements:</span></span>

- <span data-ttu-id="eed67-104">Windows 10 x64 build 1809 eller nyere installeres på enheden.</span><span class="sxs-lookup"><span data-stu-id="eed67-104">Windows 10 x64 build 1809 or later is installed on the device.</span></span>
- <span data-ttu-id="eed67-105">Antimalware-klientversion 4.18.2009.7 eller nyere installeres.</span><span class="sxs-lookup"><span data-stu-id="eed67-105">Anti-malware client version 4.18.2009.7 or later is installed.</span></span>
- <span data-ttu-id="eed67-106">Enheden er **en af** følgende:</span><span class="sxs-lookup"><span data-stu-id="eed67-106">The device is **one** of these:</span></span>
    
    - <span data-ttu-id="eed67-107">Azure Active Directory (Azure AD) forbundet</span><span class="sxs-lookup"><span data-stu-id="eed67-107">Azure Active Directory (Azure AD) joined</span></span>
    - <span data-ttu-id="eed67-108">Hybrid Azure AD forbundet</span><span class="sxs-lookup"><span data-stu-id="eed67-108">Hybrid Azure AD joined</span></span>
    - <span data-ttu-id="eed67-109">AAD registreret</span><span class="sxs-lookup"><span data-stu-id="eed67-109">AAD registered</span></span>

- <span data-ttu-id="eed67-110">Hvis du vil gennemtvinge politikhandlinger, skal du sørge for, at Microsoft Chromium Edge-browseren er installeret på slutpunktsenheden.</span><span class="sxs-lookup"><span data-stu-id="eed67-110">To enforce policy actions, make sure Microsoft Chromium Edge browser is installed on the endpoint device.</span></span>

<span data-ttu-id="eed67-111">Du kan finde yderligere krav til implementering af Endpoint DLP i Introduktion til [forebyggelse af datatab i slutpunkt.](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints)</span><span class="sxs-lookup"><span data-stu-id="eed67-111">For additional requirements for deploying Endpoint DLP, see [Get started with Endpoint data loss prevention](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).</span></span>