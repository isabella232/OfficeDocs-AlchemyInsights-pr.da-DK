---
title: Konfigurere og validere udeladelser for MDATP på en Linux-computer
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
ms.openlocfilehash: 4fad0a513f7c6d2f0337019488a4055c25e1650d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744539"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a><span data-ttu-id="820c6-102">Konfigurere og validere udeladelser for MDATP på en Linux-computer</span><span class="sxs-lookup"><span data-stu-id="820c6-102">Configure and validate exclusions for MDATP on a Linux machine</span></span>

<span data-ttu-id="820c6-103">Du kan udelade visse filer, mapper, processer og proces åbne filer fra MDATP-scanninger.</span><span class="sxs-lookup"><span data-stu-id="820c6-103">You can exclude certain files, folders, processes, and process-opened files from MDATP scans.</span></span> <span data-ttu-id="820c6-104">Udeladelse er med til at forhindre forkert registrering af software og filer, der er unikke eller tilpasset din organisation.</span><span class="sxs-lookup"><span data-stu-id="820c6-104">Exclusions help prevent incorrect detection of software and files unique or customized to your organization.</span></span> <span data-ttu-id="820c6-105">Udeladelse er også med til at afhjælpe problemer med ydeevnen, der skyldes MDATP.</span><span class="sxs-lookup"><span data-stu-id="820c6-105">Exclusions also help mitigate performance problems caused by MDATP.</span></span>

<span data-ttu-id="820c6-106">Hvis du vil have mere at vide, [skal du se Konfigurere og validere udeladelser for MDATP til Linux.](https://go.microsoft.com/fwlink/?linkid=2144517)</span><span class="sxs-lookup"><span data-stu-id="820c6-106">To learn more, see [Configure and validate exclusions for MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="820c6-107">De udeladelser, der er beskrevet i denne artikel, gælder ikke for andre funktioner i MDATP til Linux, herunder registrering af slutpunkter og svar (EDR).</span><span class="sxs-lookup"><span data-stu-id="820c6-107">The exclusions described in this article don't apply to other capabilities of MDATP for Linux, including endpoint detection and response (EDR).</span></span> <span data-ttu-id="820c6-108">Filer, som du udelader ved hjælp af de metoder, der er beskrevet i denne artikel, kan stadig udløse EDR-beskeder og andre registreringsfunktioner.</span><span class="sxs-lookup"><span data-stu-id="820c6-108">Files that you exclude by using the methods described in this article can still trigger EDR alerts and other detection capabilities.</span></span>
