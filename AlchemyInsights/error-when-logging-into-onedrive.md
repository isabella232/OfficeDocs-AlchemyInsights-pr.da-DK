---
title: 0x8004de40, når du starter OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813646"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="2350a-102">0x8004de40, når du starter OneDrive</span><span class="sxs-lookup"><span data-stu-id="2350a-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="2350a-103">Hvis du modtager en fejlmeddelelse **om 0x8004de40** når du logger på OneDrive, skal du genstarte computeren, mens du har forbindelse til dit arbejds- eller skoledomæne.</span><span class="sxs-lookup"><span data-stu-id="2350a-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="2350a-104">Hvis du får vist denne fejl efter genstart, kan du prøve dette, mens du har forbindelse til dit arbejds- eller skoledomæne:</span><span class="sxs-lookup"><span data-stu-id="2350a-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="2350a-105">Klik på Start, og **skriv cmd** eller **kommandoprompt** i søgefeltet, højreklik på appen kommandoprompt, og **vælg Kør som administrator.**</span><span class="sxs-lookup"><span data-stu-id="2350a-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator**.</span></span> <span data-ttu-id="2350a-106">Hvis du bliver bedt om at angive en administratoradgangskode eller en bekræftelse, skal du skrive adgangskoden eller klikke på **Tillad.**</span><span class="sxs-lookup"><span data-stu-id="2350a-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow**.</span></span>  

2. <span data-ttu-id="2350a-107">I vinduet Kommandoprompt skal du **skrive dsregcmd /leave**  og vente på, at kommandoen fuldføres.</span><span class="sxs-lookup"><span data-stu-id="2350a-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="2350a-108">Skriv derefter **dsregcmd /join,** og vent på, at kommandoen fuldføres.</span><span class="sxs-lookup"><span data-stu-id="2350a-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="2350a-109">Genstart computeren.</span><span class="sxs-lookup"><span data-stu-id="2350a-109">Reboot your computer.</span></span>
