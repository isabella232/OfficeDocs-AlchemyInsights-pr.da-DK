---
title: Fix 0x8004de40 fejl i OneDrive
ms.author: pebaum
author: pebaum
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 48b29f57763ca22a71a23b2afddcac0e8e8a95db
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052031"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="4c1f0-102">Fix 0x8004de40 fejl i OneDrive</span><span class="sxs-lookup"><span data-stu-id="4c1f0-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="4c1f0-103">Hvis du får en 0x8004de40-fejl med OneDrive:</span><span class="sxs-lookup"><span data-stu-id="4c1f0-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="4c1f0-104">Genstart den berørte computer, mens du har forbindelse til dit Acitve Directory-domæne.</span><span class="sxs-lookup"><span data-stu-id="4c1f0-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="4c1f0-105">Hvis en genstart ikke løser problemet, kan du fjerne joinforbindelse og tilslutte din enhed igen fra Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4c1f0-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="4c1f0-106">**Bemærk**: du bør være på virksomhedens netværk, mens du udfører disse trin.</span><span class="sxs-lookup"><span data-stu-id="4c1f0-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="4c1f0-107">Udfør ikke disse trin, når du ikke kan oprette forbindelse til virksomhedens infrastruktur (f. eks. under rejser).</span><span class="sxs-lookup"><span data-stu-id="4c1f0-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="4c1f0-108">Åbn en kommandoprompt med administratorrettigheder.</span><span class="sxs-lookup"><span data-stu-id="4c1f0-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="4c1f0-109">Hvis du vil åbne en kommandoprompt med administratorrettigheder, skal du klikke på- **Start**, højreklikke på **kommandoprompt**og derefter klikke på **Kør som administrator**.</span><span class="sxs-lookup"><span data-stu-id="4c1f0-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="4c1f0-110">Skriv *dsregcmd/Leave* , og tryk på **Enter**.</span><span class="sxs-lookup"><span data-stu-id="4c1f0-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="4c1f0-111">Skriv *dsregcmd/join* , når du er færdig, og tryk på **Enter**.</span><span class="sxs-lookup"><span data-stu-id="4c1f0-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="4c1f0-112">Luk kommandoprompten, når du er færdig.</span><span class="sxs-lookup"><span data-stu-id="4c1f0-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="4c1f0-113">Genstart computeren, og log på OneDrive.</span><span class="sxs-lookup"><span data-stu-id="4c1f0-113">Reboot the computer, and log into OneDrive.</span></span>