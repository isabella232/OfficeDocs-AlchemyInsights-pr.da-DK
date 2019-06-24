---
title: Rette fejl i 0x8004de40 i OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133971"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="f9319-102">Rette fejl i 0x8004de40 i OneDrive</span><span class="sxs-lookup"><span data-stu-id="f9319-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="f9319-103">Hvis du modtager fejlmeddelelsen 0x8004de40 med OneDrive:</span><span class="sxs-lookup"><span data-stu-id="f9319-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="f9319-104">Genstart computeren, mens du har forbindelse til din atkiv Directory-domæne.</span><span class="sxs-lookup"><span data-stu-id="f9319-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="f9319-105">Hvis en genstart ikke løser problemet, ophæve dit medlemskab og slutte enheden fra Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f9319-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="f9319-106">**Bemærk**: Du skal være på virksomhedens netværk, mens du udfører disse trin.</span><span class="sxs-lookup"><span data-stu-id="f9319-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="f9319-107">Ikke udføre disse trin, når du ikke kan oprette forbindelse til din virksomheds infrastruktur (for eksempel, mens du rejser).</span><span class="sxs-lookup"><span data-stu-id="f9319-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="f9319-108">Åbn en kommandoprompt.</span><span class="sxs-lookup"><span data-stu-id="f9319-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="f9319-109">For at åbne en kommandoprompt, klik på - **Start**, højreklik på **kommandoprompt**og derefter klikke på **Kør som administrator**.</span><span class="sxs-lookup"><span data-stu-id="f9319-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="f9319-110">Skriv *dsregcmd /leave* , og tryk på **Enter**.</span><span class="sxs-lookup"><span data-stu-id="f9319-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="f9319-111">Når du er færdig, kan du skrive *dsregcmd /join* og tryk på **Enter**.</span><span class="sxs-lookup"><span data-stu-id="f9319-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="f9319-112">Når du er færdig, kan du lukke kommandoprompten.</span><span class="sxs-lookup"><span data-stu-id="f9319-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="f9319-113">Genstart computeren, og log ind OneDrive.</span><span class="sxs-lookup"><span data-stu-id="f9319-113">Reboot the computer, and log into OneDrive.</span></span>