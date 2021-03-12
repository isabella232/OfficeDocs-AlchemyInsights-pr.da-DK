---
title: Fejlfinding af MDATP-installationsproblemer på en Mac
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744659"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a><span data-ttu-id="d099e-102">Fejlfinding af MDATP-installationsproblemer på en Mac</span><span class="sxs-lookup"><span data-stu-id="d099e-102">Troubleshoot MDATP installation problems on a Mac</span></span>

<span data-ttu-id="d099e-103">Hvis manuel installation mislykkes, **viser** installationsguiden oversigtssiden følgende fejl:</span><span class="sxs-lookup"><span data-stu-id="d099e-103">If manual installation fails, the **Summary** page of the installation wizard shows the following error:</span></span>

<span data-ttu-id="d099e-104">"Der opstod en fejl under installationen.</span><span class="sxs-lookup"><span data-stu-id="d099e-104">"An error occurred during installation.</span></span> <span data-ttu-id="d099e-105">Installationsprogrammet stødte på en fejl, der forårsagede, at installationen mislykkedes.</span><span class="sxs-lookup"><span data-stu-id="d099e-105">The Installer encountered an error that caused the installation to fail.</span></span> <span data-ttu-id="d099e-106">Kontakt softwareproducenten for at få hjælp."</span><span class="sxs-lookup"><span data-stu-id="d099e-106">Contact the software manufacturer for assistance."</span></span>

<span data-ttu-id="d099e-107">I MDM-installationer viser siden også en generisk installationsfejl.</span><span class="sxs-lookup"><span data-stu-id="d099e-107">For MDM deployments, the page shows a generic installation failure, too.</span></span>

<span data-ttu-id="d099e-108">Selvom vi ikke viser nøjagtige fejl til slutbrugere, beholder vi en logfil med installationsprocessen i **/Library/Logs/Microsoft/mdatp/install.log.**</span><span class="sxs-lookup"><span data-stu-id="d099e-108">Although we don't display exact errors to end users, we keep a log file with installation progress, in **/Library/Logs/Microsoft/mdatp/install.log**.</span></span> <span data-ttu-id="d099e-109">Hver installationssession føjes til denne logfil.</span><span class="sxs-lookup"><span data-stu-id="d099e-109">Each installation session appends to this log file.</span></span> <span data-ttu-id="d099e-110">Hvis du kun vil have output fra den seneste installationssession, skal du bruge `sed` .</span><span class="sxs-lookup"><span data-stu-id="d099e-110">To output the last installation session only, use `sed`.</span></span>

<span data-ttu-id="d099e-111">Du kan få mere at vide [under Fejlfinding af installationsproblemer for Microsoft Defender ATP til Mac.](https://go.microsoft.com/fwlink/?linkid=2144615)</span><span class="sxs-lookup"><span data-stu-id="d099e-111">To learn more, see [Troubleshoot installation issues for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span></span>
