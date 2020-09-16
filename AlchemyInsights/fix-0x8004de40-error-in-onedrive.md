---
title: Ret 0x8004de40-fejl i OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745124"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="99212-102">Ret 0x8004de40-fejl i OneDrive</span><span class="sxs-lookup"><span data-stu-id="99212-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="99212-103">Hvis du modtager en 0x8004de40-fejl med OneDrive:</span><span class="sxs-lookup"><span data-stu-id="99212-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="99212-104">Genstart den berørte computer, mens du har forbindelse til dit Acitve-katalog domæne.</span><span class="sxs-lookup"><span data-stu-id="99212-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="99212-105">Hvis en genstart ikke løser problemet, kan du afbryde og genoprette forbindelsen til din enhed fra Azure AD.</span><span class="sxs-lookup"><span data-stu-id="99212-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="99212-106">**Bemærk**: du skal være på dit virksomhedsnetværk, mens du udfører disse trin.</span><span class="sxs-lookup"><span data-stu-id="99212-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="99212-107">Du skal ikke udføre disse trin, når du ikke kan oprette forbindelse til virksomhedens infrastruktur (f. eks. under rejser).</span><span class="sxs-lookup"><span data-stu-id="99212-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="99212-108">Åbn en kommandoprompt med administratorrettigheder.</span><span class="sxs-lookup"><span data-stu-id="99212-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="99212-109">Hvis du vil åbne en kommandoprompt med administratorrettigheder, skal du klikke på **Start**, højreklikke på **kommandoprompt**og derefter klikke på **Kør som administrator**.</span><span class="sxs-lookup"><span data-stu-id="99212-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="99212-110">Skriv *dsregcmd/Leave* , og tryk på **Enter**.</span><span class="sxs-lookup"><span data-stu-id="99212-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="99212-111">Når du er færdig, skal du skrive *dsregcmd/join* og trykke på **Enter**.</span><span class="sxs-lookup"><span data-stu-id="99212-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="99212-112">Når du er færdig, skal du lukke kommandoprompten.</span><span class="sxs-lookup"><span data-stu-id="99212-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="99212-113">Genstart computeren, og log på OneDrive.</span><span class="sxs-lookup"><span data-stu-id="99212-113">Reboot the computer, and log into OneDrive.</span></span>