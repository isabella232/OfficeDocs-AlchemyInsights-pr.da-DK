---
title: 0x8004de40-fejl ved start af OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823016"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="58ccf-102">0x8004de40-fejl ved start af OneDrive</span><span class="sxs-lookup"><span data-stu-id="58ccf-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="58ccf-103">Hvis du modtager en fejl **0x8004de40** , når du logger på OneDrive, skal du genstarte computeren, mens du har forbindelse til dit arbejds-eller skole domæne.</span><span class="sxs-lookup"><span data-stu-id="58ccf-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="58ccf-104">Hvis du får denne fejl, når du har genstartet, kan du prøve dette, mens du har forbindelse til dit arbejds-eller skole domæne:</span><span class="sxs-lookup"><span data-stu-id="58ccf-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="58ccf-105">Klik på Start, og Skriv **cmd** eller **kommandoprompt**  i søgefeltet, Højreklik på appen kommandoprompt, og vælg  **Kør som administrator** .</span><span class="sxs-lookup"><span data-stu-id="58ccf-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator** .</span></span> <span data-ttu-id="58ccf-106">Hvis du bliver bedt om at angive en administratoradgangskode eller en bekræftelse, skal du skrive adgangskoden eller klikke på **Tillad** .</span><span class="sxs-lookup"><span data-stu-id="58ccf-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow** .</span></span>  

2. <span data-ttu-id="58ccf-107">I kommando prompt vinduet skal du skrive **dsregcmd/Leave**  og vente på, at kommandoen fuldføres.</span><span class="sxs-lookup"><span data-stu-id="58ccf-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="58ccf-108">Skriv derefter **dsregcmd/join** , og vent på, at kommandoen fuldføres.</span><span class="sxs-lookup"><span data-stu-id="58ccf-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="58ccf-109">Genstart computeren.</span><span class="sxs-lookup"><span data-stu-id="58ccf-109">Reboot your computer.</span></span>
