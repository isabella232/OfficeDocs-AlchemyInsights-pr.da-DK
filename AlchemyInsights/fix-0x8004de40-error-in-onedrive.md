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
ms.openlocfilehash: d436184bdc0e283db217ea734fb2c8e05f85b4e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525053"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="cecf0-102">Rette fejl i 0x8004de40 i OneDrive</span><span class="sxs-lookup"><span data-stu-id="cecf0-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="cecf0-103">Hvis du modtager fejlmeddelelsen 0x8004de40 med OneDrive:</span><span class="sxs-lookup"><span data-stu-id="cecf0-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="cecf0-104">Genstart computeren, mens du har forbindelse til din atkiv Directory-domæne.</span><span class="sxs-lookup"><span data-stu-id="cecf0-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="cecf0-105">Hvis en genstart ikke løser problemet, ophæve dit medlemskab og slutte enheden fra Azure AD.</span><span class="sxs-lookup"><span data-stu-id="cecf0-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="cecf0-106">**Bemærk**: Du skal være på virksomhedens netværk, mens du udfører disse trin.</span><span class="sxs-lookup"><span data-stu-id="cecf0-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="cecf0-107">Ikke udføre disse trin, når du ikke kan oprette forbindelse til din virksomheds infrastruktur (for eksempel, mens du rejser).</span><span class="sxs-lookup"><span data-stu-id="cecf0-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="cecf0-108">Åbn en kommandoprompt.</span><span class="sxs-lookup"><span data-stu-id="cecf0-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="cecf0-109">For at åbne en kommandoprompt, klik på - **Start**, højreklik på **kommandoprompt**og derefter klikke på **Kør som administrator**.</span><span class="sxs-lookup"><span data-stu-id="cecf0-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="cecf0-110">Skriv *dsregcmd /leave* , og tryk på **Enter**.</span><span class="sxs-lookup"><span data-stu-id="cecf0-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="cecf0-111">Når du er færdig, kan du skrive *dsregcmd /join* og tryk på **Enter**.</span><span class="sxs-lookup"><span data-stu-id="cecf0-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="cecf0-112">Når du er færdig, kan du lukke kommandoprompten.</span><span class="sxs-lookup"><span data-stu-id="cecf0-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="cecf0-113">Genstart computeren, og log ind OneDrive.</span><span class="sxs-lookup"><span data-stu-id="cecf0-113">Reboot the computer, and log into OneDrive.</span></span>