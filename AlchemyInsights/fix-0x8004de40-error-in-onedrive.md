---
title: Ret 0x8004de40-fejl i OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716022"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="3c331-102">Ret 0x8004de40-fejl i OneDrive</span><span class="sxs-lookup"><span data-stu-id="3c331-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="3c331-103">Hvis du får vist en 0x8004de40-fejl med OneDrive:</span><span class="sxs-lookup"><span data-stu-id="3c331-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="3c331-104">Genstart den berørte computer, mens den er tilsluttet Acitve Directory-domænet.</span><span class="sxs-lookup"><span data-stu-id="3c331-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="3c331-105">Hvis en genstart ikke løser problemet, skal du fjerne forbindelsen til din enhed og slutte sig til din enhed fra Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3c331-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="3c331-106">**Bemærk:** Du skal være på virksomhedens netværk, mens du udfører disse trin.</span><span class="sxs-lookup"><span data-stu-id="3c331-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="3c331-107">Udfør ikke disse trin, når du ikke kan oprette forbindelse til virksomhedens infrastruktur (f.eks. under rejsen).</span><span class="sxs-lookup"><span data-stu-id="3c331-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="3c331-108">Åbn en kommandoprompt med en forhøjet kommando.</span><span class="sxs-lookup"><span data-stu-id="3c331-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="3c331-109">Hvis du vil åbne en kommandoprompt med administrator, skal du klikke på - **Start**, højreklikke på **Kommandoprompt**og derefter klikke på **Kør som administrator**.</span><span class="sxs-lookup"><span data-stu-id="3c331-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="3c331-110">Skriv *dsregcmd /leave,* og tryk på **Enter**.</span><span class="sxs-lookup"><span data-stu-id="3c331-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="3c331-111">Skriv *dsregcmd /join,* når den er fuldført, og tryk på **Enter**.</span><span class="sxs-lookup"><span data-stu-id="3c331-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="3c331-112">Når kommandoprompten er fuldført, skal du lukke den.</span><span class="sxs-lookup"><span data-stu-id="3c331-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="3c331-113">Genstart computeren, og log på OneDrive.</span><span class="sxs-lookup"><span data-stu-id="3c331-113">Reboot the computer, and log into OneDrive.</span></span>